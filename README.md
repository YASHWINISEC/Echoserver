# Echoserver
Echo server and client using python socket

## DATE: 22.02.2025

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
## CLIENT
```
import socket
HOST,PORT = '127.0.0.1',65432
with socket.create_connection((HOST,PORT)) as s:
    s.sendall(b'Yashwini M, 212223230249')
    print(f'Received: {s.recv(1024)!r}')
```
## SERVER
```
import socket 
HOST,PORT = '127.0.0.1',65432
with socket.create_server((HOST,PORT)) as s:
    conn,add = s.accept()
    with conn: 
        print(f'Connected by{add}')
        while data :=conn.recv(1024):
            conn.sendall(data)
```

## OUTPUT:
![image](https://github.com/user-attachments/assets/5941ea10-bf22-4d8c-9ee1-0f6357e9b368)

## RESULT:
The program is executed successfully
