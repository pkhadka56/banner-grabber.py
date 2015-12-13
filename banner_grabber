#!/usr/bin/env python

import socket
import sys

def redBanner(ip,port):
    try:
        socket.setdefaulttimeout(2)
        s=socket.socket()
        s.connect((ip,port))
        banner=s.recv(1024)
        return banner
    except Exception, e:
        print "[-] Error" + str(e)
def main():
    ip1=sys.argv[1]
    port=21
    banner1=redBanner(ip1,port)
    if banner1:
        print "[+]" + ip1 + ":" + banner1

if __name__=='__main__':
    main()
