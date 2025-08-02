# MultiThreaded vs SingleThreaded Java Server

This project demonstrates the difference between a **Single Threaded Server** and a **Multi Threaded Server** using Java's `ServerSocket` and `Socket` APIs.

The goal is to showcase how multi-threading allows a server to handle multiple clients concurrently, compared to a single-threaded approach that blocks further requests until the current one is handled.

---

## 📂 Project Structure

```
MultiThreadServer/
├── single-thread/        # Contains single-threaded server and client
│   ├── SingleThreadServer.java
│   └── SingleThreadClient.java
├── multi-thread/         # Contains multi-threaded server and client
│   ├── MultiThreadServer.java
│   └── MultiThreadClient.java
└── README.md
```

---

## 🚀 Getting Started

### ✅ Requirements
- Java 8 or higher
- Any IDE (like IntelliJ, Eclipse) or terminal for running `.java` files

---

## 💡 How It Works

### 🧵 SingleThreadedServer
- Accepts one client at a time.
- Each client must wait for the previous one to disconnect before being served.
- Simpler to implement, but not scalable.

### 🧵 MultiThreadedServer
- Spawns a new thread for each client connection.
- Can serve multiple clients **simultaneously**.
- More efficient for concurrent requests.

---

## 🔨 How to Run

### 1. Compile the Server and Client
```bash
javac SingleThreadServer.java
javac SingleThreadClient.java

javac MultiThreadServer.java
javac MultiThreadClient.java
```

### 2. Run the Server
```bash
java SingleThreadServer
# or
java MultiThreadServer
```

### 3. Run the Clients (in different terminals or threads)
```bash
java SingleThreadClient
# or
java MultiThreadClient
```

---

## 📊 Output Comparison

### Single Threaded
<img width="1366" height="768" alt="Screenshot (416)" src="https://github.com/user-attachments/assets/85341243-2871-47e0-8b76-7ef669018518" />
<img width="1366" height="768" alt="Screenshot (417)" src="https://github.com/user-attachments/assets/ae3f70db-ab40-459d-af28-23a6a8ba8d4f" />
<img width="1366" height="768" alt="Screenshot (418)" src="https://github.com/user-attachments/assets/65b40517-ad21-4c5e-9b0f-6e02e148dce8" />


### Multi Threaded
<img width="1366" height="768" alt="Screenshot (414)" src="https://github.com/user-attachments/assets/3843fba0-d3e7-4255-b3f8-1a98d584a535" />
<img width="1366" height="768" alt="Screenshot (415)" src="https://github.com/user-attachments/assets/fc5bdc96-28f7-44a7-8d3b-df3a98482f15" />





## 📚 Concepts Covered

- Java `ServerSocket` and `Socket` APIs
- Basic Networking in Java
- Multi-threading using `Thread` and `Runnable`
- Concurrent client handling

---

## 📌 Use Cases

- Understanding how scalable web servers work
- Learning socket programming and thread handling in Java
- Simulating real-world server environments

---


