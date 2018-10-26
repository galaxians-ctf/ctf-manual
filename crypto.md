## Cryptography

```
sudo apt install bsdgames
```

**Tools**

*Classical*

|What|Link|
|----|----|
|Geocaching Toolbox (many classic crypto decoders)  | [http://www.geocachingtoolbox.com/index.php](http://www.geocachingtoolbox.com/index.php)|
|Substitution Cipher Fiddle| http://ba.net/util/cipher2/cipher.html |
|Substitution Cipher Autosolver| http://www.quipqiup.com/index.php |
|ROT cipher (caesar) decoder (outputs all possible rotations)| [http://planetcalc.com/1434/](http://planetcalc.com/1434/)|
|Rail fence cipher decoder| [http://rumkin.com/tools/cipher/railfence.php](http://rumkin.com/tools/cipher/railfence.php) |
|Bacon cipher decoder| [http://rumkin.com/tools/cipher/baconian.php](http://rumkin.com/tools/cipher/baconian.php) |
|Vigenere cipher decoder| [http://www.guballa.de/vigenere-solver](http://www.guballa.de/vigenere-solver) |
|Polybius cipher breaker| http://www.dcode.fr/polybius-cipher |

*Modern*

|What|Link|
|----|----|
|Prime factorization (using database)| [factordb.com](http://factordb.com)|
|factordb CLI + python library | [pypi](https://pypi.org/project/factordb-pycli/) [github](https://github.com/ryosan-470/factordb-pycli)|
|RSA calculator| [https://www.cs.drexel.edu/~introcs/Fa11/notes/10.1_Cryptography/RSA_Express_EncryptDecrypt.html](https://www.cs.drexel.edu/~introcs/Fa11/notes/10.1_Cryptography/RSA_Express_EncryptDecrypt.html) |
|RSA worksheet| [https://www.cs.drexel.edu/~introcs/Fa11/notes/10.1_Cryptography/RSAWorksheetv4d.html](https://www.cs.drexel.edu/~introcs/Fa11/notes/10.1_Cryptography/RSAWorksheetv4d.html)|
|RSA python lib | [https://pypi.python.org/pypi/rsa](https://pypi.python.org/pypi/rsa)|
|Discrete logarithm calculator| [http://www.alpertron.com.ar/DILOG.HTM](http://www.alpertron.com.ar/DILOG.HTM) |

*Hashing*

|What|Link|
|----|----|
|Online Hash database | [https://hashkiller.co.uk/](https://hashkiller.co.uk/)|
|John the Ripper| ubuntu apt tool, use Jumbo version for extra functionality [http://www.openwall.com/john/](http://www.openwall.com/john/)|

```
MD5 - 32 characters
SHA1 - 40 characters
```

**Documentation**

*Classical*

|What|Link|
|----|----|
| Rail Fence Cipher | [wikipedia](https://en.wikipedia.org/wiki/Rail_fence_cipher)|
| Scytale cipher | [scytale cipher](http://en.wikipedia.org/wiki/Scytale)|

*Modern*

*Hashing*
GOST hashing algorithm:  [http://en.wikipedia.org/wiki/GOST_%28hash_function%29](http://en.wikipedia.org/wiki/GOST_%28hash_function%29)

**Tips and Tricks**

```console
$ echo 'hello, world' | rot13
uryyb, jbeyq
$ echo 'hello, world' | caesar 1
ifmmp, xpsme
```


