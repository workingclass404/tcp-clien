# import socket

target_host = "www.google.com"
target_port = 80

#create a socket object
clien = socket.socket (socket,AF_INET, socket.SOCK STREAM)

#connect the clien
clien.send(GET /HTTP/1.1\r,\nHost :google.com\r\n\r\n")

# receive some data
response = clien.recv(4096)

print response
