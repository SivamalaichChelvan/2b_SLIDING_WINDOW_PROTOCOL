# 2b IMPLEMENTATION OF SLIDING WINDOW PROTOCOL
## AIM:
To implement a Sliding Window Protocol.
## ALGORITHM:
1. Start the program.
2. Get the frame size from the user
3. To create the frame based on the user request.
4. To send frames to server from the client side.
5. If your frames reach the server it will send ACK signal to client
6. Stop the Program
## PROGRAM
### CLIENT SIDE:
```
1. Start
2. Create a socket using TCP.
3. Bind the socket to localhost and port 8002.
4. Listen for incoming connections.
5. Accept the connection request from the server.
6. Read the number of frames (N) to be sent.
7. Create a list of frames from 0 to N−1.
8. Read the window size (W).
9. Initialize starting index i = 0.
10. Repeat until all frames are sent:
     •Send W frames starting from index i.
     •Wait for acknowledgment from the server.
11. If acknowledgment is received:
     •Move the window forward by W frames. 
     •Stop after all frames are transmitted.
12. End
```
### SERVER SIDE:
```
1. Start
2. Create a socket using TCP.
3. Connect to the client using localhost and port 8002.
4. Repeat:
   •Receive a frame window from the client.
   •Display the received frames.
   •Send acknowledgment back to the client.
5. Continue until transmission ends.
6. Close the connection.
7. End
```
## OUTPUT:
<img width="1225" height="371" alt="image" src="https://github.com/user-attachments/assets/6165152e-b81b-4a3f-bc03-8233ef48b4e6" />

## RESULT:
Thus, python program to perform stop and wait protocol was successfully executed.
