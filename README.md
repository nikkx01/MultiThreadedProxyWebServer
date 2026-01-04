# Multi-Threaded HTTP Proxy Server in C (With & Without Cache)

## Author
Nikhil Anand

## Project Overview
This project implements a multi-threaded HTTP proxy server in C that acts as an intermediary between client browsers and web servers. The proxy is capable of handling multiple client requests concurrently using POSIX threads and includes an optional caching mechanism to improve performance for repeated requests.

The project is designed as a system-level networking application for learning and demonstrating core concepts of Computer Networks and Operating Systems.

---

## Features
- Multi-threaded client handling using POSIX threads
- HTTP request parsing implemented manually
- Proxy server with and without caching support
- Improved response time using cached responses
- Thread-safe shared resources using mutex locks
- Modular code structure for easy extension

---

## Technologies Used
- C Programming Language
- Socket Programming (TCP/IP)
- POSIX Threads (pthreads)
- HTTP Protocol
- Linux / macOS Environment

---

## Project Structure
.
├── proxy_server_with_cache.c
├── proxy_server_without_cache.c
├── proxy_parse.c
├── proxy_parse.h
├── Makefile
└── README.md

---

## How to Build and Run

### Prerequisites
- GCC Compiler
- Linux or macOS (Windows via WSL supported)
