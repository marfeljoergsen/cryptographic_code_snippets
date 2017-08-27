# Cryptographic test repository

This repository contains some small Python crypto-tools I've worked with.


## Getting Started

The program is very easy to use. The "plain.txt" file is an example of something you want to be encrypted using the "many-time-pad"-method, which is rather unsecure compared to the one-time-pad. The objective is to investigate a method to attack a stream cipher where the key is used many times. After running, the program will output the "cipher.txt"-file.

In the last part of the program the "cipher.txt"-file will be used with a cryptographic attack, hence the results will be written to "result.txt". The user can change the "encLines/crackLines" variable to ignore (some) lines, hence changing the difficulty of the algorithm.


### Prerequisites

This is a small program. It uses Python3 and imports os, binascii. These variables can be changed:


```
    inFile="plain.txt"
    ciphFile="cipher.txt"
    attFile="attack.txt"
    encLines=999
    crackLines=999
```


### Results

A comparison of the original "plain.txt" and the "attack.txt" is shown below.

![Comparing "plain.txt" with "attack.txt"](./comparison_with_plainTxt.png?raw=true "Comparison")

In a future version it is a good idea to allow the user to manually fix the target plaintext (it is often obvious what the plain text is even though some characters are incorrect). The program should then output the corresponding cipher key. The idea is to add more tools/scripts about cryptography later.


### Suggested background reading
* http://toc.cryptobook.us/
* http://shoup.net/ntb/ntb-v2.pdf


## Authors

* **Martin Felix Jørgensen**


## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
