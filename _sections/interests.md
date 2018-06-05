---
title: Interests
name: interests
image: images/interests.png
rank: 2
---
This page lists some of my interests and organizations I have been involved
with. It is split into two major categories, [technical](#technical) and
[personal](#personal). The technical section contains my interests that relate
to technical fields, while the personal section contains my more creative or
activity-based interests.

### Technical
- [Applied Cybersecurity Club](#applied-cyber)
  + [Leadership](#applied-cyber-leadership)
  + [Projects](#applied-cyber-projects)
  + [Competitions](#applied-cyber-competitions)

### Personal
- [Photography](#photography)
- [The Outdoors](#outdoors)
- [Traveling](#traveling)

-------------------------------------------------------------------------------

## Technical

### [Applied Cybersecurity Club][applied-cyber-website] ![Applied Cyber Logo][applied-cyber-logo]
{: #applied-cyber}

The [Stanford Applied Cybersecurity Club][applied-cyber-website] has been a
large part of my undergraduate career. As one of the leaders of the club, I
have helped run several major workshops and events, while also working on
interesting programming projects relating to computer security.

#### Leadership
{: #applied-cyber-leadership}

Over the past two years, I have been involved in running the Applied Cyber club.
![Club Leadership][applied-cyber-leadership]
This past year, I was one of the core leadership members, responsible for
deciding on club events, managing club projects, and deciding the long-term
plans for the club. We have held a number of successful events this year,
including participating in several competitions, many workshops and talks
focusing on interesting aspects of computer security, and the start of several
significant security projects.

#### Projects
{: #applied-cyber-projects}

One of my major responsibilities for the club is running and managing different
security-focused projects that the club is working on. Below is a quick
description of the ongoing (public) projects the club is working on, and how
they aim to solve some security problem.

- **Firewall Rulest Parser:**
One major problem with modern firewall systems is that due to the sheer number
of rules, old and outdated rules can remain in the firewall. This represents
a non-trivial security risk for enterprises, and this project aims to turn
a complex firewall ruleset into a reachability graph, allowing network operators
to quickly determine if there are outdated or incorrect rules.
- **OSSFuzz:**
Google launched the OSSFuzz project to integrate and fuzz open source projects,
with the aim of finding security vulnerabilities. We spent several months
integrating the Perl-Compatible Regular Expression (PCRE) library into this
project, and these contributions should be integrated fairly soon.
- **Raft in SGX:**
This project is still in the initial stages, but aims to implement the Raft
distributed consensus protocol inside Intel's SGX environment. Additionally,
we are implementing this protocol in Rust, with the aim of reducing the
algorithm's susceptibility to Byzantine failures.

#### Competitions
{: #applied-cyber-competitions}

As part of the Applied Cyber club, I have been involved in several computer
security competitions. We have competed in both the Collegiate Cyber-Defense
Competition (CCDC) and the Collegiate Pen-Testing Competition (CPTC).
![CPTC victory][cptc_victory_picture]
The club has participated in CCDC for three seasons, and this last year the
club participated in CPTC for the first time, [winning first place
nationally.][cptc_victory_news_article] I have been on the CCDC and CPTC teams
every year the club has participated, and have found the experience extremely
valuable for giving a broad overview of the real, practical security challenges
organizations face. This has allowed me to better understand and reason about
how security research and systems design can help solve real-world security
problems.

-------------------------------------------------------------------------------

## Personal

### Photography
{: #photography}

One of my more creative passions is photography. I greatly enjoy taking photos,
as it allows me to seek out beautiful moments in the world that I normally
overlook. While I enjoy the photographs themselves, I find the process of taking
pictures even more rewarding and enjoyable. As a consequence, I have not
uploaded many of my photographs, although that is slowly changing.

Note that the background for this website and all of the banner images are
photographs that I have taken.

### The Outdoors
{: #outdoors}

My other large passion is the outdoors. Having grown up in Washington State,
![Tahoe skiing][skiing_photo]
I had the opportunity to spend a large portion of my youth in the woods and
doing outdoor activities. I greatly enjoy both backpacking and hiking, and
have spent many days exploring the Cascade Mountains and sections of the
Pacific Crest Trail. I am also a fairly avid skier, and have skied throughout
Washington, California, Colorado, and Canada.

### Traveling
{: #traveling}



[applied-cyber-logo]: {{ "/images/applied_cyber_logo.png" | absolute_url }}
{:style="float: right; margin-right: 7px; margin-top: 7px; width: 20%; height: 20%"}
[applied-cyber-website]: https://applied-cyber.stanford.edu/
{:target="\_blank"}
[applied-cyber-leadership]: {{ "/images/leadership.png" | absolute_url }}
{:style="float: left; margin-right: 7px; margin-top: 7px; width: 40%; height: 40%"}

[cptc_victory_picture]: {{ "/images/cptc_victory.png" | absolute_url }}
{:style="float: right; margin-right: 10px; margin-top: 10px; width: 40%; height:40%"}
[cptc_victory_news_article]: https://www.mercurynews.com/2017/11/15/computer-security-stanford-team-wins-national-contest/
{:target="\_blank"}

[skiing_photo]: {{ "/images/skiing_photo.png" | absolute_url }}
{:style="float: left; margin-right: 10px; margin-top: 10px; width: 30%; height:30%"}
