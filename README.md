This is the challenge we built for the first [frida-wars](https://sec-r.et/).

Credits for the awesome work to [@jeanbmar](https://github.com/jeanbmar) [@bhargavhegde001](https://github.com/bhargavhegde001) [@veronicapablo](https://github.com/veronicapablo) [@AkshayJainG](https://github.com/AkshayJainG) and [@iGio90](https://github.com/iGio90)

The goal is to read from memory a String with that format: 
**{secRet-[xxxxxxxxxxxxxxxx]}**. Our mission is to protect it and make the code use it as normal app do nowadays with tokens and stuff.

We ensure, as per competition rule, that the flag is built in memory when an obvious action (like clicking a button) is perfomed by the user and no external tools are altering the execution. Target is built for arm64 devices.


#### Guidelines
If you need some help or you want to read how we built it or need guidelines to solve it, open the [challenge details notes](CHALLENGE_DETAILS.md)

#### Solutions

* [norsecode](https://gist.github.com/jeanbmar/49b2425e240f3c47d1deda62643fe021)

* our own - [quackme](https://gist.github.com/jeanbmar/08da8ad764d5f5611fa2c438b6efe4a5)
