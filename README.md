# 3a.CREATION FOR ECHO CLIENT AND ECHO SERVER USING TCP SOCKETS
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

### CLIENT :
```

# NAME : BALAJI.A
# REG NO : 212223040023


import socket 
s=socket.socket() 
s.connect(('localhost',8000)) 
while True:
    msg=input("Client > ") 
    s.send(msg.encode()) 
    print("Server > ",s.recv(1024).decode())
```

### SERVER :
```

# NAME : Vinodhini K
# REG NO : 212223230245

import socket
s=socket.socket()
s.connect(('localhost',8000))
while True:
 print(s.recv(1024).decode())
 s.send("Acknowledgement Recived".encode())
```

## OUPUT :

![image](https://github.com/user-attachments/assets/e052a5a5-6151-4e1b-9a09-53ad94d2fb0a)

## RESULT :
Thus, the python program for creating Echo Client and Echo Server using TCP Sockets Links 
was successfully created and executed.
