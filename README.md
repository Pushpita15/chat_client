## A simple Chat application

This project demonstrates the use of sockets in networking to build connections for data communication , the project is built using pythin 
and Tiknter is used for the GUI . 
The project consists of a main.py script that serves as the entry point, 
and several modules inside the src directory, including ask_ip.py, ask_mode.py, client_mode.py, and server_mode.py. 
These modules help in handling different aspects of the chat client and server application.

## Server Mode (server_mode.py)

  1. This script represents the server side of the chat application.
  2. It creates a GUI window using Tkinter for the server to interact with.
  3. The server's IP address and default port (5000) are displayed
  4. It initializes a SOCKETS object , which manages the server's socket connections.
  5. The server binds to the specified port, listens for incoming connections,
      and spawns a new thread to handle each connected client.
  6. Messages recieved from clients are displayed in the chat history panel.
## Client Mode(client_mode.py)

  1. This script represents the client side of the chat application.
  2. It creates a GUI window using Tkinter where clients can enter the server's IP address and port number.
  3. It also has ipnut fields for sending text messages and displaying chat history.
  4. The client initializes a SOCKETS object to manage socket connection.
  5. It connects to the server using the provided IP and port.
  6. Messages sent by the client are displayed in blue , and messages recieved rom the server or other clients are displayed in green.

## SOCKETS Class
  1. This class encapsulates the socket related functionality for both the client and server.
  2. It manages socket creation , binding(server), connecting(client),sending, and recieving messages.
  3. Messages are exchanged in UTF-8 encoding.
  4. Recieved messages are displayed in the chat history panel.
## Script: main.py

The main.py script is the entry point of our application. 
It imports modules for asking the user for the operation mode (ask_mode), client functionality (client_mode), and server functionality (server_mode). 
Depending on the user's choice, it launches either the client or server interface.
