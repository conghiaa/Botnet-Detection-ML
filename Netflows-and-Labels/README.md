__Note__: the sample database set used in the example is ...
## Goals
* Process pcap files to obtain [netflow](https://en.wikipedia.org/wiki/NetFlow)  records and other properties (features) related to each netflow for be used later
>
* Labels those records to differentiate various types of traffic (e.g. normal, background or botnet)

<strong>Netflow Type</strong>

They should be either of type __uni-directional__ and __bi-directional__. We choose bidirectional type because it has some advantages over the other one:

> "First, they solve the issue of differentiating between the client and the server, second they include more information and third they include much more detailed labels"

Each flow is defined by a tuple __(Source IP, Source Port, Destinaton IP, Destination Port, Protocol)__

<strong>Netflow Features</strong>
>

<strong>Labeling scheme</strong>
>

## Tools
1. [Argus](https://qosient.com/argus/)
>
2. Argus-clients: ar and ralabel
>

## Workflow
1. Configure argus.conf file (in other words, we're configuring netflow type)
>
2. Configure ra.conf file(to format csv output)
>
3. Configure ralabel.conf file (for labeling engine)
>
4. Generate labeled netflow file in csv format
>

## References
http://geek00l.blogspot.com/2008/01/network-flow-uni-directional-vs-bi.html
