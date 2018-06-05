---
title: Projects
name: projects
image: images/projects.png
rank: 1
---
Below are some of the major projects I've worked on. They are split into two
main categories - [research](#research) and [implementation](#implementation),
and the lists below contain a quick description and a link to each project.

### [Research](#research)
Research projects are projects I've worked on that are either particularly
novel, or resulted in a publishable contribution or result.
- [The Tock Operating System:](#tockos) A secure, embedded OS in Rust
- [SOSP 2017 Tutorial:](#sosp2017) Tutorial for Tock at SOSP
- [6LoWPAN:](#6lowpan) Research on the 6LoWPAN protocol

### [Implementation](#implementation)
My implementation projects are projects that have less of an academic focus, and
are generally implementations of already published work.
- [Senior Project:](#senior-project) Wireless application updating
- [CS 244B Project:](#cs244b) Distributed protocol for eventual consistency
- [CS 241 Project:](#cs241) Low-power water quality measurement system

-------------------------------------------------------------------------------

## Research
For research projects, the bulk of my work has focused on networking for
embedded systems. These projects are all either part of existing research
projects or are projects that have resulted in interesting, publishable work.

### The Tock Operating System ![Tock logo][tock_logo]
{: #tockos}
[website][tock_website_button]
[code][tock_code]

The [Tock research project][tock_website] is an embedded operating
system written in Rust. The goal of the project is to improve the security of
low-power, IoT devices by leveraging Rust's compile-time guarantees.


My work on this project has focused on the networking stack, and I am
implementing a UDP/IPv6/6LoWPAN stack on Tock, which is slowly making its way
into the mainstream kernel. You can check out my code for this project on my
fork on [GitHub](https://github.com/ptcrews/tock).

### SOSP 2017 Tutorial ![SOSP logo][sosp_2017_logo]
{: #sosp2017}
[tutorial][sosp_2017_tutorial]

As part of my involvement with the Tock project, I helped run a tutorial on
using Tock at SOSP 2017 in Shanghai. While there, we presented the Tock
operating system to other systems researchers, giving a quick tutorial on how
to use and interface with the operating system. By introducing other researchers
to the Tock platform, we hoped to encourage other researchers and institutions
to use Tock in the future.

### 6LoWPAN ![6LoWPAN logo][6lowpan_logo]
{: #6lowpan}
[poster][6lowpan_poster]

As part of my work on Tock, I spent several months implementing the 6LoWPAN
protocol, which is a compression scheme for wireless, low-power IPv6 networks.
Although much of the implementation work was included in Tock, some of the
challenges I ran into helped to motivate a paper. This paper analyzed and
detailed interoperability challenges of 6LoWPAN, and how the protocol seems to
be unnecessarily complex. This paper was submitted to Sensys 2018.

-------------------------------------------------------------------------------

## Implementation

For implementation projects, most of my projects have focused on embedded
systems, networking, and distributed systems. These project differ from my
research projects as they are either re-implementations of already published
work, or are projects that did not produce significantly novel results.
A collection of my work is listed below.

### Senior Project
{: #senior-project}
[code][senior_project_code]

For my senior project, I am implementing the [Deluge protocol][deluge_paper]
on the Tock platform. This protocol is used for updating binaries in low-power
wireless networks, and allows for the efficient dissemination of binaries to
multiple listening nodes. In addition to standard single-binary Deluge, this
project aims to multiplex the protocol and allow for multiple binaries to be
updated simultaneously.

This project will be completed by June 2018.

### CS 244B Project
{: #cs244b}
[paper][cs244b_final_paper]
[code][cs244b_code]
[presentation][cs244b_presentation]

![CS 244B image][cs244b_image]

For my final project in CS 244B (Distributed Systems), my group implemented a
modified version of the [Trickle algorithm][trickle_paper] which aims for
eventual consistency in low-power wireless networks. As part of our
modifications, we enabled some portion of nodes in the network to completely
enter sleep mode, rather than requiring all nodes remain in the listen state.
This improved the power efficiency of the network, while still retaining the
eventually consistent distributed system property.

### CS 241 Project ![CS241 image][cs241_image]
{: #cs241}
[Build Your Own][cs241_tutorial]

For my final project in CS 241 (Embedded Systems), my group created a low-power
wireless water quality monitor system. We implemented a test-bed on the STM
Nucleo microcontroller, which was aimed at allowing different sensors to be
plugged into the board. The system would then periodically transmit sensor
measurements over GSM. We published an online tutorial demonstrating how we
implemented this project.

[tock_website]: https://www.tockos.org/
{:target="\_blank"}
[tock_logo]: {{ "/images/tock_logo.svg" | absolute_url }}
{:style="float: right;margin-right: 7px;margin-top: 7px;"}
[tock_website_button]: https://www.tockos.org/
{:class="button special icon fa-link" target="\_blank"}
[tock_code]: https://github.com/ptcrews/tock
{:class="button special icon fa-github" target="\_blank"}

[sosp_2017_tutorial]: {{ "/docs/sosp2017tutorial.pdf" | absolute_url }}
{:class="button special icon fa-download" target="\_blank"}
[sosp_2017_logo]: {{ "/images/sosp_2017_logo.jpg" | absolute_url }}
{:style="float: right;margin-right: 7px;margin-top: 7px;width:30%;height:30%;"}

[6lowpan_poster]: {{ "/docs/sixlowpan_poster.pdf" | absolute_url }}
{:class="button special icon fa-download" target="\_blank"}
[6lowpan_logo]: {{ "/images/6lowpan_logo.png" | absolute_url }}
{:style="float: right;margin-right: 7px;margin-top: 7px;width:25%;height:25%;"}

[senior_project_code]: https://github.com/ptcrews/tock/tree/deluge_protocol
{:class="button special icon fa-github" target="\_blank"}
[deluge_paper]: https://web.stanford.edu/class/cs244e/papers/deluge.pdf
{:target="\_blank"}

[cs244b_image]: {{ "/images/cs244b_project.png" | absolute_url }}
{:style="float: right;margin-right: 7px;margin-top: 7px;width:50%; height:50%;"}
[cs244b_final_paper]: {{ "/docs/cs244b_project.pdf" | absolute_url }}
{:class="button special icon fa-download" target="\_blank"}
[cs244b_code]: https://github.com/ptcrews/tock/tree/cs244b_trickle
{:class="button special icon fa-github" target="\_blank"}
[cs244b_presentation]: {{ "/docs/cs244b_presentation.pdf" | absolute_url }}
{:class="button special icon fa-download" target="\_blank"}
[trickle_paper]: http://csl.stanford.edu/~pal/pubs/trickle-nsdi04.pdf
{:target="\_blank"}

[cs241_tutorial]: http://www.instructables.com/id/Low-Energy-River-Quality-Monitor/
{:class="button special icon fa-link" target="\_blank"}
[cs241_image]: {{ "/images/cs241_image.png" | absolute_url }}
{:style="float: right;margin-right: 7px;margin-top: 7px;width: 30%; height: 30%;"}
