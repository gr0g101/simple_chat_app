# simple_chat_app
It is a simple chat application which uses both, asymmetric and symmetric encryption to operate. The main motivation behind the project was that, I wanted to learn more about cryptography and its implementation, so I decided to create this project.

The application was developed with python 3.8.3. The server and the client exchanging the public keys. Then the server uses RSA encryption to encrypt a random generated session key and it will be shared with the client. After this process the client will decrypt it with its own private key and uses that secret to encryp/decrypt messages using AES in CFB mode. The server can handle multiple clients connected, and it doesn't keep the messages.

For improvement I will add digital signature verification to the project as well.
