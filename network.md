# Network

```
sudo apt install wireshark tshark
```


## Tools

Wireshark (packet dissection): ubuntu apt tool [https://www.wireshark.org/](https://www.wireshark.org/)


## Documentation

## Tips and Tricks

Wireshark -> export objects -> HTTP

### Selecting data with tshark

- Select http requests: (`-Y http.response` for all responses, or `-Y http` for everything)

	```
	$ tshark -r data.pcap -Y http.request
	 4   0.001196 192.168.3.129 → 192.168.3.128 HTTP 387 GET / HTTP/1.1
	17  12.370383 192.168.3.129 → 192.168.3.128 HTTP 522 POST /login HTTP/1.1  (application/x-www-form-urlencoded)
	27  12.434002 192.168.3.129 → 192.168.3.128 HTTP 480 GET /admin HTTP/1.1
	43  14.662211 192.168.3.129 → 192.168.3.128 HTTP 486 GET /logout HTTP/1.1
	54  14.673355 192.168.3.129 → 192.168.3.128 HTTP 424 GET / HTTP/1.1
	68  37.234879 192.168.3.129 → 192.168.3.128 HTTP 542 POST /login HTTP/1.1  (application/x-www-form-urlencoded)[Packet size limited during capture]
	```

- See all fields available for http requests (`-Tjson` also works)

	```
	$ tshark -r data.pcap -Y http.request -T pdml
	<packet>
	  <proto name="geninfo" pos="0" showname="General information" size="387">
		<field name="num" pos="0" show="4" showname="Number" value="4" size="387"/>
		<field name="len" pos="0" show="387" showname="Frame Length" value="183" size="387"/>
		<field name="caplen" pos="0" show="387" showname="Captured Length" value="183" size="387"/>
		<field name="timestamp" pos="0" show="Jul  8, 2018 22:56:55.848235000 CEST" showname="Captured Time" value="1531083415.848235000" size="387"/>
	```

- See just the POSTed data:

	```
	$ tshark -r data.pcap -Y http.request -Tfields -e http.file_data

	user=jimmy&password=p4ssw0rd



	user=admin&password=picoCTF{n0ts3cur3_894a6546}
	```
