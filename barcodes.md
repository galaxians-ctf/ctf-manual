# Barcodes

## List of barcodes

- [Linear barcodes](https://en.wikipedia.org/wiki/Barcode#Linear_barcodes)
- [2D barcodes](https://en.wikipedia.org/wiki/Barcode#Matrix_(2D)_barcodes)



## Specifications

- [QR code format](https://en.wikipedia.org/wiki/QR_cod://en.wikipedia.org/wiki/QR_code)
- [Data Matrix](https://en.wikipedia.org/wiki/Data_Matrix)


## Tools

| tool           | description                            | link                                   |
| -------------- | -------------------------------------- | -------------------------------------- |
| Barcode reader | Online barcode scanner                 | https://www.onlinebarcodereader.com/   |
| qrtools        | Python library for QR codes            | https://github.com/primetang/qrtools   |
| QRazyBox       | QR code analysis and recovery toolkit  | https://merricx.github.io/qrazybox/    |


## Manually decoding

- [video] [decoding QR code by hand](https://www.youtube.com/watch?v=KA8hDldvfv0)
- [video] [decoding data matrix by hand](https://www.youtube.com/watch?v=w0xVd2xXySo)

## QR Codes

![](/images/qr-code-explained.jpg)

**Tools**

```
sudo apt-get install zbar-tools
```

**Documentation**

|What|Link|
|----|----|
|QR-code format description | [http://www.ucreative.com/articles/what-is-a-qr-code-and-how-does-it-work/](http://www.ucreative.com/articles/what-is-a-qr-code-and-how-does-it-work/) |
|QR-code format description | [wikipedia](https://en.wikipedia.org/wiki/QR_code) |
|Decoding QR-codes by hand | https://www.youtube.com/watch?v=KA8hDldvfv0 |
|Detailed/Interactive Tutorial | [https://www.nayuki.io/page/creating-a-qr-code-step-by-step](https://www.nayuki.io/page/creating-a-qr-code-step-by-step) |

**Tips**

Reading QRcodes from command line

```
zbarimg myqrimage.png
```
