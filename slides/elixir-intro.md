# Elixir for starters

<small>by</small>

<medium>Fabian Król & Maciek Talaśka</medium>

<small>23rd January 2019 Wrocław, Poland</small>
----

## What is Elixir?

#### yet another language?
====

### Elixir is:

* functional
* concurrent
* general purpose
* running on top of **BEAM (Erlang VM)**
* **uses actor model**
====

### Elixir History

* created by Jose Valim, Rails core team member
* "how to make Ruby concurrent"
* BEAM + Ruby syntax = Elixir
* erlang's core ideas + ruby's developers first approach

Note:
Jose: "I was member of the Rails Core Team from early 2010 to mid 2014, where I have received the Ruby Hero Award as a recognition for my work on other Open Source projects."
====

### Elixir: Erlanger perspective
- modern language
- better tooling
- big vibrant community
- opensource is in roots of Elixir
- metaprogramming, macros, ...
====

### Elixir: ruby perspective
- functional programming
- performance
- concurrency
- distribution
----




## Elixir prehistory
### aka. erlang: the most boring language
====

### BEAM
- industry battle tested
- scheduler per CPU core
- lightweight processes
- no shared memory
- process isolation
- failure isolation
====

### Actor model 101

* mathematical model of concurrent computation
* no shared state between actors
* asynchronous message passing to other actors
* actor reacts to messages
====

### erlang
- designed to build telecom systems
- OTP _Open Telecom Platform_

Note:
1. one of few programming languages designed by industry demand, not adopted by it
2. OTP is made up of three components:
    The Erlang programming language
    A set of libraries, including tools, interfaces and reusable applications
    A set of design principles and patterns describing the system’s architecture
====

### BEAM, Erlang, Elixir
- Erlang ~ Java
- Beam ~ JVM
- Elixir ~ Scala
====

### Other BEAM based languages

* LFE
* Clojerl
* alpaca
* gleam
* efene
* ephp
* joxa

<small>(source: https://github.com/llaisdy/beam_languages)</small>

Note:
1. compare BEAM growing number of languages to JVM revolution after .Net was revealed
2. if there are so many BEAM languages... why Elixir?
----


## Let's continue on Elixir...
====

### Tooling

* hex.pm - the package manager
* mix - build tool
* mix can handle all day to day development tasks

====

### Erlang in Elixir

- tooling: dialyzer, observer
- tracing: debug/trace live systems
- Elixir standard library != Erlang standard library ...
- ... but it is possible to use Erlang lib
- easy to use Erlang projects from Elixir
====

### Phoenix

* web framework
* inspired by Rails
* it is *NOT* Rails!
* uniqe: LiveView

Note:
* LiveView is not released yet (is it?)
====

### Ecto

* inspired by ActiveRecord
* inspired, but... it is *NOT* ActiveRecord for Elixir/Phoenix
* works with RDBMS
* ...and with NoSQL
====

### Nerves

* works on popular devices (Raspberry Pi)

> "Phoenix may bring jobs for Elixir today,
Nerves is about future".

====

### Elixir success stories

* Netflix
* WhatsApp\*
* SquareEnix
* bet365
* Discord

Note:
Discord is capable of handling 5M concurrent users (https://blog.discordapp.com/scaling-elixir-f9b8e1e7c29b)
WhatsApp: "They wrote their application fully in Erlang, which is compiled to same bytecode that Elixir is"
====

### Community

* the best ideas taken from Ruby community
* friendly, welcome
* open discussions, everyone is welcome
* growing fast

====

### Elixir today
- vibrant community
- Elixir borrowed from Erlang a lot...
- ...but also influences today's Erlang

====

### Elixir & Erlang popularity (USA)

<img src="slides/trends_erlang_elixir.png" >

<div style="background: white; width: 676px; margin-left: auto; margin-right: auto; margin-top: -50px;">
	<div style="padding: 10px;">
		<small>
			<font color="#f44336">Elixir</font> <font color="#2196f3">Erlang</font><br>
			<font color="black">5 years span: 2014 - 2019</font>
		</small>
	</div>
</div>

<small>(source: https://trends.google.com)</small>
====

### Elixir & Erlang popularity (World)

<img src="slides/trends_erlang_elixir_worldwide.png">

<div style="background: white; width: 665px; margin-left: auto; margin-right: auto; margin-top: -50px;">
	<div style="padding: 10px;">
		<small>
			<font color="#f44336">Elixir</font> <font color="#2196f3">Erlang</font><br>
			<font color="black">5 years span: 2014 - 2019</font>
		</small>
	</div>
</div>

<small>(source: https://trends.google.com)</small>
====


### Elixir & Erlang on TIOBE

Erlang: 50

Elixir: 50+

<small>(source: https://www.tiobe.com/tiobe-index/)</small>
Note:
Elixir could be 51st, but TIOBE list 50+ languages in alphabetical order
====

### Elixr & Erlang @ SO:

Erlang: 8341

Elixir: 562

<small>(as of: 2019-01-19)</small>

Note:
1. Erlang is much older than Elixir
2. What does that mean that there are many question? Does that mean language is hard to grasp?
3. Elixir has a very good forum (other languages are also migratinig from sites like SO)
====

### Future of Elixir & Erlang

 > **Elixir is the future of Erlang systems**
--Fabian

Note:
even ErlangSystem is doing consulting with Elixir now
----




## Is Elixir good for me...

### ...and my project
====

### Elixir is great for:

* distributed systems
* fault tolerant
* highly scalable systems
* high uptime systems
(it is not pick 2 out of 3. get **ALL**)
* prototyping

Note:
* low latency vs high throughput
====

### Elixir is good for

1. Web development (Phoenix, Ecto)
2. IoT (Nerves)
3. WebAssembly?
4. Scripting
====

### What is Elixir **not** good for?

1. Heavy computations
2. Systems programming
3. Direct hardware interaction (drivers)
4. GPGPU, realtime graphics...
5. Desktop applications

Note:
1a. You should not build HPC based on Elixir itself (short info on how to do that)
1b. NIF, interprocess communication (use for example: Rust for external processes)
----




## Starting with Elixir
====

### Learning resources
- awesome elixir: https://github.com/h4cc/awesome-elixir
- Programming Phoenix 1.4 (Chris McCord, Bruce Tate, Jose Valim)
- Programming Elixir 1.6 (Dave Thomas)
- Metaprogramming Elixir (Chros McCord)
- Elixir in Action, 2nd ed (Sasa Juric)
- The little Elixir & OTP book (Benjamin Tan Wei Hao)
- podcasts & screencasts: https://github.com/elixir-lang/elixir/wiki/Podcasts-and-Screencasts

Note:
1. Pragpub was first with Elixir books, and has many titles (probably the most)
2. (pragpub discount!)
====

### Installation

1. Get Erlang (https://www.erlang-solutions.com/resources/download.html)
2. Install Elixir (https://elixir-lang.org/install.html)
 - binary package or use version manager (asdf)
3. Install PostgreSQL (https://blog.pragtechnologies.com/phoenix/)

Note:
1. why not asdf for Erlang? (documentation)
2. why asdf for Elixir (short release cycle, super easy to update)
3. check Elixir site for more detailed info on installation
4. Why PostgreSQL?
5. Why different resource for installing PostgreSQL...
====

### Do I need an IDE for Elixir?

- Elixir is **functional**, so...
- Spacemacs + alchemist plugin
- PyCharm(!) + Elixir plugin
- Vim + alchemist.vim
- Visual Studio Code /Atom
- SublimeText3

Note:
functions = refactoring is much easier
in the past Spacemacs + alchemist was the best option (most mature)
Elixir Language Server should make it easier for any other editors/IDEs to support Elixir
====

### Where do I deploy?

* Gigalixir: https://gigalixir.com
* Heroku

----




## Summary

### what you should remember
====

### Erlang is to Java...

Beam     ~ Jvm

Erlang   ~ Java

Elixir   ~ Scala

====

### Elixir is

* functional
* concurrent
* general purpose
* running on top of **BEAM (Erlang VM)**
* **uses actor model**
====

### Elixir tech for starters

Phoenix  ~ Rails for Elixir

Ecto ~ ActiveRecord for Elixir

Nerves - IoT for Elixir

You **do not** have to learn Erlang to use Elixir

----




### Common Questions
#### (future meetings)

1. Elixir vs Kubernetes
2. Elixir vs Serverless
3. Elixir vs Cloud
4. Elixir vs Akka & Pony
5. Elixir vs Dart
----




# Thanks!

<big>https://elixir-wroclaw.github.io/</big>
----




# NETWORKING
