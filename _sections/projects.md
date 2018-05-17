---
title: Projects
name: projects
image: images/tock.png
---
Below are some of the major projects I've worked on. They are split into two
main categories - research and implementation.

## Research
For research projects, the bulk of my work has focused on networking for
embedded systems.

### [The Tock Operating System](https://www.tockos.org/) ([code](https://github.com/ptcrews/tock))

The [Tock research project](https://www.tockos.org) is an embedded operating
system written in Rust. The goal of the project is to improve the security of
low-power, IoT devices by leveraging Rust's compile-time guarantees.

![Tock logo]({{ "/images/tock_logo.svg" | absolute_url }})

My work on this project has largely been focused on the networking stack. I
am implementing a UDP/IPv6/6LoWPAN stack on Tock, which is slowly making its
way into the mainstream kernel. You can check out my code for this project
on my fork on [GitHub](https://github.com/ptcrews/tock).

### SOSP 2017 Tutorial ([tutorial]({{ "/docs/sosp2017tutorial.pdf" | absolute_url }}))

As part of my involvement with the Tock project, I helped run a tutorial on
using Tock at SOSP 2017 in Shanghai. While there, we presented the Tock
operating system to other systems researchers, giving a quick tutorial on how
to use and interface with the operating system. By introducing other researchers
to the Tock platform, we hoped to encourage other researchers and institutions
to use Tock in the future.

### 6LoWPAN ([poster]({{ "/docs/sixlowpan_poster.pdf" | absolute_url }}))

As part of my work on Tock, I spent several months implementing the 6LoWPAN
protocol, which is a compression scheme for wireless, low-power IPv6 networks.
Although much of the implementation work was included in Tock, some of the
challenges I ran into helped to motivate a paper. This paper analyzed and
detailed interoperability challenges of 6LoWPAN, and how the protocol seems to
be unnecessarily complex. This paper was submitted to Sensys 2018.

-------------------------------------------------------------------------------

## Implementation

For implementation projects, most of my projects have focused on embedded
systems, networking, and distributed systems. A collection of my work is listed
below.

### Senior Project ([code](https://github.com/ptcrews/tock/tree/deluge_protocol))

For my senior project, I am implementing the
[Deluge protocol](https://web.stanford.edu/class/cs244e/papers/deluge.pdf)
on the Tock platform. This protocol is used for updating binaries in low-power
wireless networks, and allows for the efficient dissemination of binaries to
multiple listening nodes. In addition to standard single-binary Deluge, this
project aims to multiplex the protocol and allow for multiple binaries to be
updated simultaneously.

This project will be completed by June 2018.

### CS 244B Project ([paper]({{ "/docs/cs244b_project.pdf" | absolute_url }}), [code](https://github.com/ptcrews/tock/tree/cs244b_trickle))

For my final project in CS 244B (Distributed Systems), my group implemented a
modified version of the
[Trickle algorithm](http://csl.stanford.edu/~pal/pubs/trickle-nsdi04.pdf)
which aims for eventual consistency in low-power wireless networks. As part of
our modifications, we enabled some portion of nodes in the network to completely
enter sleep mode, rather than requiring all nodes remain in the listen state.
This improved the power efficiency of the network, while still retaining the
eventually consistent distributed system property.

### CS 241 Project ([tutorial](http://www.instructables.com/id/Low-Energy-River-Quality-Monitor/))

For my final project in CS 241 (Embedded Systems), my group created a low-power
wireless water quality monitor system. We implemented a test-bed on the STM
Nucleo microcontroller, which was aimed at allowing different sensors to be
plugged into the board. The system would then periodically transmit sensor
measurements over GSM. We published an online tutorial demonstrating how we
implemented this project.