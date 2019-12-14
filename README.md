# meetups
Materials from Fuzzing Bay Area meetups

## Meetup #2 (2019-12-12)

Original event [link](https://www.eventbrite.com/e/fuzzing-bay-area-meetup-2-tickets-82684518621#).

### Talks

#### Fuzzing Adoption at Facebook

[Slides](slides/Fuzzing_Adoption_at_Facebook.pdf).
Speaker: Hasnain Lakhani ([twitter](https://twitter.com/mhlakhani), [github](https://github.com/mhlakhani)).

There are a lot of resources on how to build and scale a fuzzing platform. There’s less information on how to build a sustained, larger-scale effort to get a whole organization onboard. Over the last 12-18 months, we built a centralized platform that all teams at Facebook can use. We will cover the history/motivation behind this work, and some principles to take into account while doing this. There will be interesting anecdotes on the engineering side (e.g. the power of copy-pastable commands); and war stories from the organizational side (convincing developers to become fuzzing advocates). We will share some of the things that worked for us and why, so listeners can tweak them for their organizations.

#### Expanding the Reach of Fuzz Testing

[Slides](slides/Expanding_the_Reach_of_Fuzzing.pdf).
Speaker: Caroline Lemieux ([twitter](https://twitter.com/cestlemieux), [github](https://github.com/carolemieux)).

Recently coverage-guided fuzz testing has gained huge traction in industry and academia thanks to its scalability and bug-finding power. However, due to its random-mutation-based input generation technique, coverage-guided fuzzing cannot reach far beyond the syntax analysis stage of programs. In this talk, I will introduce several projects expanding the reach of fuzz testing. First, I will introduce our work allowing fuzz testers to find inputs triggering a wider variety of interesting (bad) behaviors, including performance bottlenecks, excess memory allocations, and exercising program diffs (PerfFuzz, FuzzFactory). Then, I will describe how our work on smartly controlling mutations---either by direct masking (FairFuzz) or by way of input generators (Zest)---helps fuzzers produce inputs that exercise (and expose bugs in) the core logic of the program.

#### Your Browser is my Fuzzer: Fuzzing Native Applications in Web Browsers

[Slides](https://github.com/jonathanmetzman/wasm-fuzzing-demo/blob/master/meetup-Fuzzing-Native-Applications-in-Browsers-With-WASM.pdf).
Speaker: Jonathan Metzman ([twitter](https://twitter.com/metzmanj), [github](https://github.com/jonathanmetzman)).

Through WebAssembly and Emscripten, many important native applications, like SQLite, can run in virtually all web browsers (including Chrome, Edge, Firefox, and Safari). This makes it possible to fuzz native applications in web browsers using familiar fuzzing tools such as libFuzzer and ASAN.

This talk will:
- Demo in-browser fuzzing on real programs like SQLite.
-- Viewers can participate by fuzzing the applications in their own browsers.
- Help users fuzz their own native applications in-browser by:
-- Releasing the tools needed to do so.
-- Teaching them how to fuzz applications in-browser.
- Explore some use cases for in-browser fuzzing.
-- In particular, how it can enable the dream of crowdsourced fuzzing.
- Explain how technologies that allow for in-browser fuzzing, such as WebAssembly, work.
-- This will be geared towards developers familiar with fuzzing and not web programming.
-- This will touch on the changes to libFuzzer that were needed to support in-browser fuzzing.


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
