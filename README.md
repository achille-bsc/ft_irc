# ft_irc

## Overview

**ft_irc** is a project from School 42 that challenges students to implement their own Internet Relay Chat (IRC) server. This project aims to deepen understanding of network programming, socket communication, and the IRC protocol while building a functional chat server that can handle multiple clients simultaneously.

## 🎯 Project Goals

- **Network Programming**: Learn socket programming and client-server architecture
- **Protocol Implementation**: Understand and implement the IRC protocol (RFC 1459)
- **Concurrency**: Handle multiple clients simultaneously using I/O multiplexing
- **C++ Development**: Apply object-oriented programming principles in C++98

## 📋 Features

### Core Functionality
- [x] TCP/IP socket communication
- [x] Multiple client connections
- [x] User authentication (nickname, username, password)
- [x] Channel management (join, part, list)
- [x] Private messaging between users
- [x] Channel messaging
- [x] Operator privileges and channel moderation

### IRC Commands Implemented
- **Connection Management**: `PASS`, `NICK`, `USER`, `QUIT`
- **Channel Operations**: `JOIN`, `PART`, `TOPIC`, `LIST`, `NAMES`
- **Communication**: `PRIVMSG`, `NOTICE`
- **Operator Commands**: `KICK`, `INVITE`, `MODE`
- **Server Information**: `PING`, `PONG`, `MOTD`

### Channel Modes
- `+i`: Invite-only channel
- `+t`: Topic restriction (only operators can change topic)
- `+k`: Channel password
- `+o`: Operator privileges
- `+l`: User limit

## 🛠️ Technical Requirements

- **Language**: C++98
- **Compilation**: No compilation errors or warnings
- **Memory Management**: No memory leaks
- **I/O Operations**: Non-blocking I/O using `poll()`, `select()`, or `epoll()`
- **Network**: TCP sockets for client-server communication

## 🚀 Getting Started

### Prerequisites
- C++ compiler (g++ or clang++)
- Make
- Unix-like operating system (Linux/macOS)

#### Basic IRC Commands Example
```
PASS mypassword
NICK alice
USER alice alice localhost :Alice Smith
JOIN #general
PRIVMSG #general :Hello everyone!
QUIT :Goodbye
```

## 📁 Project Structure

```
ft_irc/
├── includes/           # Header files
│   ├── Server.hpp
│   ├── Client.hpp
│   ├── Channel.hpp
│   └── ...
├── src/               # Source files
│   ├── main.cpp
│   ├── Server.cpp
│   ├── Client.cpp
│   ├── Channel.cpp
│   └── ...
├── Makefile          # Build configuration
└── README.md         # This file
```

## 📚 IRC Protocol Resources

- [RFC 1459 - Internet Relay Chat Protocol](https://tools.ietf.org/html/rfc1459)
- [RFC 2812 - Internet Relay Chat: Client Protocol](https://tools.ietf.org/html/rfc2812)
- [Modern IRC Client Protocol](https://modern.ircdocs.horse/)

## ⚖️ License

This project is part of the School 42 Common Core. Please respect the school's academic integrity policies.

## 🎓 School 42

This project is part of the School 42 Common Core - Circle 5.

---

*Made with ❤️ at School 42*