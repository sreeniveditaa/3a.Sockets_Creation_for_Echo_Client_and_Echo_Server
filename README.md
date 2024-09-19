# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
# DATE :
# AIM
To write a python program for creating Echo Client and Echo Server using TCP
Sockets Links.
## ALGORITHM:
1. Import the necessary modules in python
2. Create a socket connection to using the socket module.
3. Send message to the client and receive the message from the client using the Socket module in
 server .
4. Send and receive the message using the send function in socket.
## PROGRAM
### Client
```
Developed by: SREE NIVEDITAA SARAVANAN
Reg no: 212223240141
import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True: 
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```
### Server
```
import socket 
s=socket.socket() 
s.bind(('localhost',8000)) 
s.listen(5) 
c,addr=s.accept() 
while True: 
    ClientMessage=c.recv(1024).decode() 
    c.send(ClientMessage.encode())
```
## OUPUT

![{AB37556E-02F1-4DAE-878B-B60175011BA0}](https://github.com/user-attachments/assets/96d0eb54-4d48-4370-9ac5-9612cecea18e)

![{FD1D692B-26CE-4A59-9944-5626141CD538}](https://github.com/user-attachments/assets/d954f5db-7053-4b03-9d0d-78e6ec19f21a)


## RESULT
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
