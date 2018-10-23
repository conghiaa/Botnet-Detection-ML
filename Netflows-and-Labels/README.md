## Goals
* Process pcap files to obtain [netflow](https://en.wikipedia.org/wiki/NetFlow)  records and other properties (features) related to each netflow for be used later

* Labels those records to differentiate various types of traffic (e.g. normal, background or botnet)

__Netflow Type__

They should be either of type __uni-directional__ and __bi-directional__. We choose bidirectional type because it has some advantages over the other one:

> First, they solve the issue of differentiating between the client and the server, second they include more information and third they include much more detailed labels


## References
http://geek00l.blogspot.com/2008/01/network-flow-uni-directional-vs-bi.html
