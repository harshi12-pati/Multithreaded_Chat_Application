# Multithreaded_Chat_Application

**COMPANY:** CODTECH IT SOLUTIONS

**NAME:** HARSHITHA PATI

**INTERN ID:** CT08DM1234

**DOMAIN:** JAVA PROGRAMMING

**DURATION:** 8 WEEKS

**MENTOR:** NEELA SANTOSH

---

**DESCRIPTION:**

As part of my internship at **CodTech**, I was assigned to build a **Multithreaded Chat Application** using **Java sockets**. The main objective was to design and develop a functional client-server communication system that could handle multiple users concurrently. This application simulates a basic real-time chat room where clients can send and receive messages through a centralized server. The project showcases key concepts in **socket programming**, **multithreading**, and **TCP-based communication**, and was built entirely using Java’s core libraries.

This task not only helped improve my technical skills in network programming but also gave me experience in managing multiple clients and synchronizing their communication efficiently through threads.

#

 **What the Tool Does:**

The chat application is divided into two core components: a **Server** and multiple **Clients**.

* The **Server** listens on a specified port for incoming connections and remains active throughout the session.
* Each **Client** establishes a connection with the server and starts an independent two-way communication channel.
* A **dedicated thread** is created for each client, enabling smooth and concurrent message exchange.
* Messages from one client are received by the server and then **broadcast** to all other connected clients.
* The server also keeps track of active users and can handle new user connections or disconnections in real-time.

This system creates a group chat environment where multiple users can interact without interrupting each other’s messages, ensuring a seamless chat experience.

#

 **How I Built It:**

To develop this application, I used **standard Java libraries** only, which made the system efficient and portable without relying on external dependencies.

Key components included:

* `ServerSocket` and `Socket` for establishing and managing connections.
* `Thread` and `ExecutorService` to handle multithreading for multiple clients.
* `BufferedReader` and `PrintWriter` to handle input/output streams efficiently.
* A loop in the server continuously listens for connections and creates new threads for each connected client.
* Shared messages are managed centrally by the server and sent to all clients using synchronized logic.

The architecture is clean and modular:

* **`ChatServer`**: Main server class that listens for clients and handles broadcasting.
* **`ClientHandler`**: Runnable class that manages each client’s input/output streams and thread lifecycle.
* **`ChatClient`**: A user-side application to connect, send, and receive messages.

#

 **Handling Errors and Edge Cases:**

* I included **robust error handling** using `try-catch-finally` blocks to handle unexpected I/O failures.
* The server detects when a client disconnects and removes the client from the active user list to maintain system integrity.
* Stream and socket closures are safely managed using **try-with-resources**, preventing memory leaks.
* Input validation ensures that empty or invalid messages don’t disrupt the chat session or affect other users.

#

**Tools and Environment:**

* **Java SE 8+**
* **IntelliJ IDEA** for development
* **JDoodle** for quick testing in an online environment
* No third-party libraries used—built entirely with Java’s standard networking and I/O packages

#

 **What I Learned:**

Through this project, I gained hands-on experience with:

* Building real-time network applications using **Java socket programming**
* Managing concurrency through **multithreading**
* Designing scalable **client-server architectures**
* Writing clean, maintainable, and modular code
* Implementing effective **error handling** for network-related operations

This project significantly improved my confidence in developing networked applications. It also deepened my understanding of how communication works at the socket level, which is essential for backend systems, collaborative tools, and distributed applications.

---
**OUTPUT :** 

![Image](https://github.com/user-attachments/assets/62762f92-4b0b-4db2-9cfc-6e13725b0737)
