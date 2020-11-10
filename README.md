# simple_chat_app
It is a simple chat application which uses both, asymmetric and symmetric encryption to operate. The main motivation behind the project was that, I wanted to learn more about cryptography and its implementation, so I decided to create this application.

For development python version 3.8.3 had been used. The server and the client exchanging the public keys. Then the server uses RSA encryption to encrypt a random generated session key and it will be shared with the client. After this process the client will decrypt it with its own private key and uses that secret to encryp/decrypt messages using AES in CFB mode. The server can handle multiple clients connected, and it doesn't keep the messages.

Usage:

The server can be started using one parameter which should be the port number on which the server will listen
- python3 server.py -p 4444

The client has three parameters, -s server ip, -p server port number, -u username of the user
- python3 client.py -s 127.0.0.1 -p 4444 -u gr0g101

The server can be terminated by typing 'TERMINATE' on the console.
The client can be terminated by typing 'EXIT' on the console.

For improvement I will add digital signature verification to the project.
