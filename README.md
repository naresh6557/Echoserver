# Ex1-Echoserver
Echo server and client using python socket

# AIM:

To develop a simple webserver to serve html programming pages.

## DESIGN STEPS:

### Step 1:

Design of echo server and client using python socket

### Step 2:

Implementation using Python code

### Step 3:

Testing the server and client 

## PROGRAM:
## CLIENT:
```
import socket
HOST, PORT = '127.0.0.1', 65432
with socket.create_connection((HOST, PORT)) as s:
    s.sendall(b'Naresh kumar R, 212224040213')
    print(f'Received: {s.recv(1024)!r}')
```

## SERVER:
```
import socket
host,port='127.0.0.1',65432
with socket.create_server((host,port))as s:
    conn,addr=s.accept()
    with conn:
        print(f'connected by {addr}')
        while data :=conn.recv(1024):
            conn.sendall(data)
```

## OUTPUT:
## CLIENT:
![image](https://github.com/user-attachments/assets/453d7a74-9544-4500-bb76-1d06482c0713)

## SERVER:
![image](https://github.com/user-attachments/assets/31ba61ea-1030-4a2d-8361-dce249269a64)



## RESULT:
The program is executed successfully
