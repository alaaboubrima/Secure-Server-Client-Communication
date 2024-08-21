# Secure Server-Client Communication Project

## Project Overview

This project demonstrates secure communication between a server and multiple clients using RSA encryption. The server handles multiple client connections, stores client information, and securely exchanges messages with each connected client.

## Features

1. **Secure Message Exchange**:
    - The server exchanges encrypted messages with each client using RSA encryption to ensure secure communication.
  
2. **Client Information Logging**:
    - The server maintains a log file that records the names and IP addresses of all connected clients.

3. **Message Handling**:
    - Each client receives RSA-encrypted messages from the server, stores them in a local file, and sends an acknowledgment back to the server with its details.

## Project Structure

- **server.ipynb**: Contains the server code that handles multiple client connections, encrypts messages using RSA, logs client details, and manages message exchanges.
- **client1.ipynb**: Client 1 script that connects to the server, receives and stores RSA-encrypted messages, and sends acknowledgments.
- **client2.ipynb**: Client 2 script with similar functionality as Client 1 but operates as a separate entity.

## How to Run

1. **Start the Server**:
    - Run `server.ipynb` to start the server. Then choose a client so the server will listen for incoming client connection.
  
2. **Connect Clients**:
    - Run `client1.ipynb` and `client2.ipynb` to connect clients to the server. The client that the server chose will receive RSA-encrypted messages from the server, store them, and send back an acknowledgment.

3. **Check Logs**:
    - The server creates a log file with the names and IP addresses of connected clients. This file is updated as new clients connect.

## Requirements

- Python 3.x
- Jupyter Notebook
- Libraries ("RSA", "Socket", "Time")
## Usage Notes

- Ensure that the server is running before starting the clients.
- Clients should be connected from different IPs for testing multiple client functionality.
- The project can be extended to support more clients or use different encryption methods.

## Conclusion

This project successfully demonstrates secure communication between a server and multiple clients using RSA encryption. It ensures that all messages are securely transmitted, and client information is properly logged and acknowledged.