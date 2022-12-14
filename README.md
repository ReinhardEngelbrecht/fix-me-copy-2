# [Fix-me](https://github.com/tkmaseleme/Fix-Me/blob/master/documentation/fixme.en.pdf)

A stock exchange simulation using trading algorithms, networking and socket implementations

![Build](https://github.com/tkmaseleme/Fix-Me/workflows/Build/badge.svg)

The [Marking Sheet](https://github.com/tkmaseleme/Fix-Me/blob/master/documentation/fixme.markingsheet.pdf) we are marked against.

## About

### What is [Fix-me](https://github.com/tkmaseleme/Fix-Me/blob/master/documentation/fixme.en.pdf)

One rainy day, you find out about the FIX Protocol and decide that you want to make a lot of money on the stock exchange by using your programming skills and making the computer do the heavy lifting for you. In order to do this you need some hardcore, lightning fast, enterprise grade tools. You will use these tools to simulate electronic trading and experiment with trading algorithms.

### Things I've learnt building [Fix-me](https://github.com/tkmaseleme/Fix-Me/blob/master/documentation/fixme.en.pdf)

- Use [non blocking sockets](https://www.developer.com/java/data/what-is-non-blocking-socket-programming-in-java.html#:~:text=Non-blocking%20Sockets%20in%20Java,used%20for%20blocking%20socket%20programming.&text=Non-blocking%20sockets%2C%20on%20the,hand%2C%20are%20non-sequential.)
- Use the [java executor framework](https://stackabuse.com/concurrency-in-java-the-executor-framework/) for message handling
- [Multi-module](https://www.baeldung.com/maven-multi-module) Maven build
- [FIX](https://www.onixs.biz/fix-protocol.html#:~:text=The%20Financial%20Information%20eXchange%20\(FIX,entities%20including%20trade%20allocation%2C%20order) protocol
- And a whole lot more

## Usage

Compile: `mvn clean package`

Run: 
```
java -jar router/target/router.jar
java -jar market/target/market.jar
java -jar broker/target/broker.jar
```
