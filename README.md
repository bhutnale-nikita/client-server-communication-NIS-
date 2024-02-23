# Chat Application Documentation

## Server Side

### File: chatserver.java

#### Description:
- This file contains the code for the server-side of the chat application.
- It establishes a connection with the client, sends and receives messages, and applies a simple encryption technique to the messages before sending them.

#### Components:
- `msg_area`: JTextArea to display received messages.
- `msg_text`: JTextField to input messages.
- `msg_send`: JButton to send messages.
- `msg_org`: JTextArea to display original messages sent by the user.
- `jLabel1`, `jLabel2`, `jLabel3`: JLabels for labeling various sections of the GUI.

### File: chatclient.java

#### Description:
- This file contains the code for the client-side of the chat application.
- It connects to the server, sends and receives messages, and also applies a simple encryption technique similar to the server.

#### Components:
- `msg_area`: JTextArea to display received messages.
- `msg_text`: JTextField to input messages.
- `msg_send`: JButton to send messages.
- `msg_org`: JTextArea to display original messages sent by the user.
- `jLabel1`, `jLabel2`, `jLabel3`: JLabels for labeling various sections of the GUI.

## Encryption Technique:
- Both server and client use a simple Caesar cipher encryption technique to encrypt messages before sending them. The shift value used for encryption is 2.

## Instructions for Use:
1. Run the `chatserver.java` file to start the server.
2. Run the `chatclient.java` file to start the client.
3. Type messages in the client's `msg_text` field and click on the "send" button to send messages.
4. Messages will be displayed in the respective `msg_area` fields of both client and server after encryption/decryption.

## Additional Notes:
- The application uses Java Swing for the GUI.
- Communication between the server and client is established using sockets.
- Ensure that both the server and client are running on the same network for proper communication.

