# 🚀 Multithreaded Web Server

## 🌐 Overview
This project is a **Multithreaded Web Server** implemented in Java, designed to handle multiple client requests concurrently. It includes three different implementations:

1. 🧵 **SingleThreaded Server** - Handles one request at a time.
2. ⚡ **MultiThreaded Server** - Creates a new thread for each incoming request.
3. 🎯 **ThreadPool Server** - Uses a fixed number of threads to manage multiple requests efficiently.

This project was tested using **Apache JMeter** to analyze performance under high request loads.

## ✨ Features
- 🏗️ **Single-threaded mode** (Processes requests sequentially)
- 🚀 **Multi-threaded mode** (Spawns a new thread per request)
- 🔄 **Thread-pool mode** (Manages threads efficiently to optimize resource usage)
- 🌍 **Handles HTTP GET requests**
- 📊 **Tested using Apache JMeter** for performance analysis

## ⚙️ Installation & Setup
### 📌 Prerequisites
- ☕ **Java 8+**
- 🛠️ **Apache JMeter** (for load testing)

### 🏃 Steps to Run
1. **Clone the repository**:
   ```bash
   git clone https://github.com/karthikeyan-ss/MultithreadedWebServer.git
   cd MultithreadedWebServer
   ```
2. **Compile the Java files**:
   ```bash
   javac -d out src/*.java
   ```
3. **Run the desired server implementation**:
   - 🧵 **SingleThreaded Server**:
     ```bash
     java -cp out SingleThreadedServer
     ```
   - ⚡ **MultiThreaded Server**:
     ```bash
     java -cp out MultiThreadedServer
     ```
   - 🎯 **ThreadPool Server**:
     ```bash
     java -cp out ThreadPoolServer
     ```

## 📈 Performance Testing with JMeter
To simulate multiple concurrent users, **Apache JMeter** was used:
1. 🏗️ Set up a **Thread Group** with 1000+ threads.
2. 🌐 Configure HTTP requests to the server.
3. 📊 Monitor CPU and memory usage.
4. 🔄 Compare the efficiency of different implementations.

## 🔍 Observations
- 🧵 The **SingleThreaded Server** struggles with high loads.
- ⚡ The **MultiThreaded Server** scales well but consumes more system resources.
- 🎯 The **ThreadPool Server** provides a balance between performance and resource usage.

## 🙌 Credits
This project was built by **Karthikeyan SS**, inspired by a **YouTube tutorial** by [AlphaDecodeX](https://github.com/AlphaDecodeX).

## 📜 License
This project is open-source and available under the **MIT License**.

---
Feel free to contribute or suggest improvements! 🚀

