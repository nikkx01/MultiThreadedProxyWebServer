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

### Steps
1. Clone the repository:
   ```bash
   git clone https://github.com/nikkx01/MultiThreadedProxyWebServer.git
   cd MultiThreadedProxyWebServer

2. Choose the version to run:

* For cached proxy:
  Update Makefile to use proxy_server_with_cache.c

* For non-cached proxy:
  Update Makefile to use proxy_server_without_cache.c

3. Compile the project:
   make

4. Run the proxy server:
   ./proxy 8080

## How to use
This is a local system-level application and is not hosted online.
1. Start the proxy server on a local port
2. Configure your browser’s proxy settings:
   * Server: 127.0.0.1
   * Port: 8080
3. Browse any HTTP website normally
4. Observe terminal logs for request handling and cache hits/misses

## Learning Outcomes
* Understanding proxy server architecture
* Hands-on experience with socket programming
* Practical use of multi-threading and synchronization
* Exposure to HTTP request/response handling
* Cache design and performance optimization