🧵 Multi-Threaded Proxy Server in C
📌 Project Overview
This project implements a multi-threaded proxy server using C and socket programming.
The proxy server sits between multiple clients and destination servers, forwarding client requests and relaying responses while handling concurrent connections efficiently using POSIX threads.
This project demonstrates practical understanding of Computer Networks, Operating Systems, and concurrent system design.
🏗️ Architecture
Client  ───▶  Proxy Server  ───▶  Target Web Server
Client  ◀───  Proxy Server  ◀───  Target Web Server
Each client connection is handled by a separate thread, allowing multiple clients to be served simultaneously.
⚙️ Features
Supports multiple clients concurrently
Implemented using TCP socket programming
Uses POSIX threads (pthreads) for multithreading
Acts as an intermediary between client and destination server
Clean modular code structure
Designed for scalability and extensibility
🛠️ Tech Stack
Language: C
Networking: BSD Sockets (TCP/IP)
Concurrency: POSIX Threads (pthreads)
Platform: Linux / macOS
📂 Project Structure
MultiThreaded-Proxy-Server/
│
├── server/
│   ├── proxy_server.c
│   ├── server_utils.h
│
├── client/
│   └── client.c
│
├── logs/
├── README.md
├── Makefile
└── .gitignore
🚀 How to Run
1️⃣ Compile the Server
gcc server/proxy_server.c -o proxy_server -lpthread
2️⃣ Start the Proxy Server
./proxy_server
3️⃣ Run the Client
gcc client/client.c -o client
./client
🧪 Testing
The proxy server can be tested using:
curl http://example.com --proxy localhost:<PORT>
📚 Concepts Used
TCP/IP Networking
Socket lifecycle (socket, bind, listen, accept)
Multithreading using pthread_create
Client-server architecture
Synchronization and concurrency handling
📈 Future Enhancements
Thread pool implementation
Request caching
HTTPS support
Logging and monitoring
Access control and authentication
🧑‍💻 Author
Nikhil Anand
Mathematics & Computing,
Delhi Technological University (DTU)
⭐ Why This Project?
This project was built to strengthen hands-on knowledge of low-level networking, multithreading, and system programming, making it suitable as a resume and interview project for software engineering roles.