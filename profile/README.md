Rust and Elixir libraries for end-to-end encrypted, mutually authenticated, secure communication.

Data, within modern distributed applications, are rarely exchanged over a single point-to-point
transport connection. Application messages routinely flow over complex, multi-hop, multi-protocol
routes — _across data centers, through queues and caches, via gateways and brokers_ — before reaching
their end destination.

Transport layer security protocols are unable to protect application messages because their protection
is constrained by the length and duration of the underlying transport connection.

Ockam is a suite of programming libraries and infrastructure that makes it simple for our applications
to guarantee end-to-end integrity, authenticity, and confidentiality of data.

We no longer have to implicitly depend on the defenses of every machine or application within the same,
usually porous, network boundary. Our application's messages don't have to be vulnerable at every point,
along their journey, where a transport connection terminates.

Instead, our application can have a strikingly smaller vulnerability surface and easily make
_granular authorization decisions about all incoming information and commands._

<hr>

## Features

* End-to-end encrypted, mutually authenticated _secure channels_.
* Key establishment, rotation, and revocation - _for fleets, at scale_.
* Identity profiles isolated by _privacy contexts_.
* Attribute-based Access Control - credentials with _selective disclosure_.
* Add-ons for a variety of operating environments, transport protocols, and _cryptographic hardware_.
* Libraries for multiple languages - _Rust, Elixir_ (more on the roadmap).

<hr>

## Learn

* [__Hello Ockam__](https://github.com/ockam-network/ockam#hello-ockam):
Write a simple example to create an encrypted secure channel between Alice and Bob. When a message is sent through
this channel it will be encrypted when it enters the channel and decrypted just before it exits the channel.
[👉](https://github.com/ockam-network/ockam#hello-ockam)

* [__Build End-to-End Encryption with Rust__](https://github.com/ockam-network/ockam/tree/develop/documentation/use-cases/end-to-end-encryption-with-rust#readme):
In this hands-on guide, we create two small Rust programs called Alice and Bob. Alice and Bob send each other
messages, over the network, via a cloud service. They mutually authenticate each other and have a cryptographic
guarantee that the integrity, authenticity, and confidentiality of their messages is protected end-to-end.
[👉](https://github.com/ockam-network/ockam/tree/develop/documentation/use-cases/end-to-end-encryption-with-rust#readme)

* [__Build End-to-End Encryption through Kafka__](https://github.com/ockam-network/ockam/tree/develop/documentation/use-cases/end-to-end-encryption-through-kafka#readme):
In this guide, we show two programs called Alice and Bob. Alice and Bob send each other messages, over
the network, via a cloud service, _through Kafka_. They mutually authenticate each other and have a
cryptographic guarantee that the integrity, authenticity, and confidentiality of their messages is protected
end-to-end. The Kafka instance, the intermediary cloud service and attackers on the network are not be able
to see or change the contents of en-route messages. The application data in Kafka is encrypted.
[👉](https://github.com/ockam-network/ockam/tree/develop/documentation/use-cases/end-to-end-encryption-through-kafka#readme)

* [__How to end-to-end encrypt all application layer communication__](https://github.com/ockam-network/ockam/tree/develop/documentation/use-cases/end-to-end-encrypt-all-application-layer-communication#readme):
In this hands-on guide, we'll create two simple Rust programs to __transparently tunnel__ arbitrary
application layer communication through Ockam's end-to-end encrypted, mutually authenticated secure channels.
These example programs are also available in a docker image so you can try them without setting up a rust
toolchain.
[👉](https://github.com/ockam-network/ockam/tree/develop/documentation/use-cases/end-to-end-encrypt-all-application-layer-communication#readme)

* [__Build a secure access tunnel to a service in a remote private network__](https://github.com/ockam-network/ockam/tree/develop/documentation/use-cases/secure-remote-access-tunnels#readme):
In this guide, we'll write a few simple Rust programs to programmatically create secure access tunnels to remote
services and devices that are running in a private network, behind a NAT. We'll then tunnel arbitrary communication
protocols through these secure tunnels.
[👉](https://github.com/ockam-network/ockam/tree/develop/documentation/use-cases/secure-remote-access-tunnels#readme)

* [__Step-by-Step Deep Dive__](https://github.com/ockam-network/ockam/tree/develop/documentation/guides/rust#readme):
In this step-by-step guide we write many small rust programs to understand the various building blocks
that make up Ockam. We dive into Node, Workers, Routing, Transport, Secure Channels and more.
[👉](https://github.com/ockam-network/ockam/tree/develop/documentation/guides/rust#readme)
