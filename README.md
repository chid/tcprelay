this code is definitely not by me.
many thanks to Hector Martin and Nikias Bassen

url: http://marcansoft.com/blog/iphonelinux/usbmuxd/

Usage
=====

```
Usage: tcprelay.py [OPTIONS] RemotePort[:LocalPort] [RemotePort[:LocalPort]]...

Options:
  -h, --help            show this help message and exit
  -t, --threaded        use threading to handle multiple connections at once
  -b KILOBYTES, --bufsize=KILOBYTES
                        specify buffer size for socket forwarding
  -s PATH, --socket=PATH
                        specify the path of the usbmuxd socket
```

Example
=======

Forwarding Remote Messages (2), SSH and VNC.

`$ python tcprelay.py -t 22:2222 333:333 5900:5900 5800:5800`