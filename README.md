README for Chat Application**

**Overview**
------------

This is a simple chat application implemented in Java. It includes a server and a client component. The server manages multiple client connections and broadcasts messages to all connected clients. The client allows users to log in, send messages, and view the list of online users.

**Components**
-------------

### Server

- **MyServer.java**: This class sets up the server and handles incoming client connections. It maintains a list of connected clients and broadcasts messages to all clients.
- **MyThread.java**: This class represents a thread that handles a single client connection. It reads messages from the client, updates the list of online users, and sends messages to all clients.

### Client

- **MyClient.java**: This class sets up the client GUI and handles user interactions. It includes buttons for sending messages, logging in, logging out, and exiting.
- **ClientThread.java**: This class represents a thread that handles the client's connection to the server. It reads messages from the server and updates the client's GUI accordingly.

**How to Run**
--------------

### Server

1. Compile the `MyServer.java` file.
2. Run the compiled `MyServer.class` file.

### Client

1. Compile the `MyClient.java` file.
2. Run the compiled `MyClient.class` file.

**Usage**
---------

### Server

- The server listens for incoming connections on port 10.
- When a client connects, the server creates a new thread to handle the connection.

### Client

- The client GUI includes buttons for sending messages, logging in, logging out, and exiting.
- Users can log in by entering their nickname.
- Users can send messages to all online users.
- Users can log out to disconnect from the server.

**Notes**
------

- This is a basic implementation and does not include error handling or advanced features.
- The server does not store user data persistently; it loses all data when it is restarted.
- The client does not handle disconnections or errors robustly.

**Acknowledgments**
----------------

This code is based on a simple chat application example and has been modified to include additional features.
