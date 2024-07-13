+++
title = 'OVT - Bandit Level 0-1'
date = 2024-07-13T20:55:01+07:00
draft = false
tags = ['overthewire','bandit']
categories = ['security']
series = ['overthewire-wargames']
+++

# Introduction

In today's connected world, cybersecurity is more important than ever. Most of our businesses and organizations are heavily reliant on IT infrastructure, so it's critical to keep it secure to ensure our society keeps functioning.

As someone who's just starting out in software development, I've learned that security is a major concern when building applications. We often see that one of the non-functional requirements is security, right? It's rarely part of our daily discussions (at least not as often as frameworks, languages, performance, etc.), but it's still one of the most important aspects for developers to consider when building software.

One of the best places to learn more is [OverTheWire Wargames](https://overthewire.org/wargames/). They have lots of games that teach us about specific topics. Each game has several levels. According to the web, they suggest starting with the [Bandit game](https://overthewire.org/wargames/bandit/). So, let's get into it.

# Steps

A brief information, we will do all activities of this game in terminal. I’m using Ubuntu on WSL2 for this game, although Windows Powershell is also fine.

## 1. Connecting to the server

Notice that you have connection information in the top left corner of the page (host and port). Use that to create SSH connection to the server with the user and password provided,

```bash
$ ssh <USER>@<HOST> -p <PORT>
```

type `yes` when asked :

```bash
...
This key is not known by any other names
Are you sure you want to continue connecting (yes/no/[fingerprint])?
```

then type the password.

## 2. Open file “readme”

As stated by the clue, the next level password is stored in a file called “readme” in home directory. You can locate it with `ls` command, and print it out to stdout with `cat` command,

```bash
$ cat readme
```

and that’s it for level 1. Dont forget to copy the password and save it somewhere as it will require you to start over if you lost it.

Lastly, you need to close the session if you want to proceed to the next level, type `exit` .
