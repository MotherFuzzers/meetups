# meetups
Materials from Fuzzing Bay Area meetups

## Meetup #1 (2019-08-22)

Original event [link](https://www.eventbrite.com/e/fuzzing-bay-area-meetup-tickets-66626376285#).

### Talks

#### Modern fuzzing of C/C++

[Slides](https://docs.google.com/presentation/d/1SxyVufvodMqV8-WIgRtZAE9gH8YSn9Rl6vIkPHk77As/edit?usp=sharing).
Speaker: Max Moroz ([twitter](https://twitter.com/dor3s), [github](https://github.com/Dor1s)).

The team that fuzzes Chrome browser, other Google products and hundreds of open source projects will give an overview of modern fuzzing tools. Learn how a trivial fuzz target can discover numerous vulnerabilities when it’s used with interchangeable fuzzing engines and runs on a fully automated fuzzing infrastructure. Nowadays, it's all available in open source and doesn't require any special skills.

#### Fuzzing APIs and web apps for fun and profit

[Slides](https://docs.google.com/presentation/d/1ec7hpiXWF5o5cTpySkeJBWNV7WsJjI5TyiPbZFcx9yY).
Speaker: Ivan Novikov ([twitter](https://twitter.com/d0znpp), [github](https://github.com/d0znpp)).

Fuzzing is a very popular security research tool for binaries, data flows, and network protocols. However, the use of fuzzing web applications and APIs has been limited. In this talk, I want to share my personal experience and recipes on how to fuzz web applications and APIs to find new vulnerabilities in a limited time frame. This talk included a detailed description of a few vulnerability types discovered initially by fuzzing, such as Memcached-injections (presented by me at BlackHat USA 2014), k-v injections and more.

#### Increasing Red Team Capabilities with Smart Fuzzing

[Slides](https://drive.google.com/file/d/1b_a85T_RS1ey6tQ2Zo7SG5N-RRhDSIJY/view?usp=sharing).
Speaker: Maksim Shudrak ([twitter](https://twitter.com/MShudrak), [github](https://github.com/mxmssh)).

The ultimate goal of any Red Team is to provide a realistic simulation of a potential adversary to highlight potential gaps and enhance security within the target company. This simulation requires a full spectrum of sophisticated skills including social engineering, networking, system security as well as malware development, reverse engineering, and vulnerability research. The latter is a crucial part of any Red Team and allows to perform perimeter penetration, privilege escalation and lateral movement using 1 and 0-day vulnerabilities found during security research. While there are many approaches to detect vulnerabilities, fuzzing remains to be #1 technique for searching memory-corruption bugs in applications written in C/C++. However, efficient fuzzing requires a lot of effort and resources from security researchers especially when we talk about Red Teaming. In this talk, we will discuss how to integrate fuzzing within offensive security program and find exploitable bugs to deliver the best security engagements.
