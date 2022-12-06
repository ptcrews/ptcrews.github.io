---
title: Projects
name: projects
rank: 4
---

## A Formal Foundation for Recoverability (2021 - Present)

I have been leading a research project collaboration between Google and
Stanford on how to design systems that can mitigate and recover from a
compromise. This work is still ongoing, and has resulted in a [poster at USENIX
Security 2022][usenix-2022-poster].

[usenix-2022-poster]: {{ "/posters/ptcrews_USENIX_Security_2022_poster.pdf" | absolute_url }}
{:class="icon fa-file-pdf" target="\_blank"}

## Tock Operating System (2017 - 2018)
[website][tock-website-button]

While a student at Stanford, I worked on the [Tock research
project][tock-website]. Tock is an embedded operating system written in Rust,
which leverages Rust's type system to provide security guarantees with low
overhead. I helped implement the 6LoWPAN protocol and networking stack in Tock.
Through this work, we discovered that other implementations of 6LoWPAN are not
interoperable, resulting in [a paper at DCOSS in 2020][dcoss-2020-paper].

[tock-website]: https://www.tockos.org/
{:class="icon solid fa-link" target="\_blank"}
[tock-website-button]: https://www.tockos.org/
{:class="button icon solid fa-link" target="\_blank"}
[dcoss-2020-paper]: https://doi.org/10.1109/DCOSS49796.2020.00027
{:class="icon solid fa-link" target="\_blank"}

## Class Projects

Below are a few major class projects I worked on while a student at Stanford.

[comment]: # TODO: Add CS356 project.

### Senior Project: Deluge Protocol on Tock
[code][senior-project-code]

For my senior project, I implemented the [Deluge protocol][deluge-paper] on the
Tock platform. This protocol is used for efficiently updating binaries in a
wireless mesh network. This project extended the single-binary Deluge to
support updating multiple binaries simultaneously.

[senior-project-code]: https://github.com/ptcrews/tock/tree/deluge_protocol
{:class="button icon solid brands fa-github" target="\_blank"}
[deluge-paper]: https://dl.acm.org/doi/10.1145/1031495.1031506
{:class="icon solid fa-link" target="\_blank"}

### CS244B: Trickle Algorithm on Tock
[paper][cs244b-final_paper]
[code][cs244b-code]
[presentation][cs244b-presentation]

![CS 244B image][cs244b-image]

For my final project in CS 244B (Distributed Systems), my group implemented a
modified version of the [Trickle algorithm][trickle-paper] which aims for
eventual consistency in low-power wireless networks. As part of our
modifications, we enabled some portion of nodes in the network to completely
enter sleep mode, rather than requiring all nodes remain in the listen state.
This improved the power efficiency of the network while still retaining
eventual consistency.

[cs244b-image]: {{ "/images/cs244b_project.png" | absolute_url }}
{:style="float: left;margin-right: 7px;margin-top: 7px;width:50%; height:50%;"}
[cs244b-final_paper]: {{ "/docs/cs244b_project.pdf" | absolute_url }}
{:class="button icon solid fa-file-pdf" target="\_blank"}
[cs244b-code]: https://github.com/ptcrews/tock/tree/cs244b_trickle
{:class="button icon solid brands fa-github" target="\_blank"}
[cs244b-presentation]: {{ "/docs/cs244b_presentation.pdf" | absolute_url }}
{:class="button icon solid fa-file-pdf" target="\_blank"}
[trickle-paper]: https://www.usenix.org/conference/nsdi-04/trickle-self-regulating-algorithm-code-propagation-and-maintenance-wireless
{:class="icon solid fa-link" target="\_blank"}

### CS 241: Low-Power Wireless Water Quality Measurement
![CS241 image][cs241-image]
[Build Your Own][cs241-tutorial]

For my final project in CS 241 (Embedded Systems), my group created a low-power
wireless water quality monitor system. We implemented a test-bed on the STM
Nucleo microcontroller, which was aimed at allowing different sensors to be
plugged into the board. The system would then periodically transmit sensor
measurements over GSM. We published an online tutorial demonstrating how we
implemented this project.

[cs241-tutorial]: http://www.instructables.com/id/Low-Energy-River-Quality-Monitor/
{:class="button icon solid fa-link" target="\_blank"}
[cs241-image]: {{ "/images/cs241_image.png" | absolute_url }}
{:style="float: right;margin-right: 7px;margin-top: 7px;width: 30%; height: 30%;"}
