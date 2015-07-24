Bindings to OpenSSL
-------------------

[![Build Status](https://travis-ci.org/jeroenooms/openssl.svg?branch=master)](https://travis-ci.org/jeroenooms/openssl)
![downloads](http://cranlogs.r-pkg.org/badges/grand-total/openssl)

OpenSSL bindings for R. Includes support for cryptographic hashing, secure RNG, base64 encoding, encryption and
creating/verifying signatures. For more information, see the vignettes:

 - [Generating Secure Random Numbers in R](https://cran.r-project.org/web/packages/openssl/vignettes/secure_rng.html) 
 - [Cryptographic Hashing in R](https://cran.r-project.org/web/packages/openssl/vignettes/crypto_hashing.html)

### OSX users

Special note for Mac: the version of OpenSSL included with OSX is a bit old (0.9.8). 
This version usually suffices but might not support the latest generation of ciphers
and algorithms. To install the most recent version of OpenSSL:

```
brew update
brew install openssl
brew link --force openssl
```

Check which version you are running (run in a fresh clean terminal):

```
openssl version -a
```

### Installation

Install from stable version from [CRAN](http://cran.r-project.org/web/packages/openssl/index.html):

```r
install.packages('openssl')
```

Or get the bleeding edge:

```r
library(devtools)
install_github("jeroenooms/openssl")
```
