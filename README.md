# ProxPy
Web Proxy with capabilities to request  HTTPv1.1, IP and URL filter, powerful CLI.

ProxPy is written in Python 3, making use of TCP sockets for communications between web browser and Web servers. For the communication of the proxy server with the logger it will do so using UDP sockets.

The application uses the select function to evade the blocking condition of certain operations with sockets. 

----

## Manual

ProxPy has two modules, the proxy server and the logger that registers the requests and responses that transpire through ProxPy.

* First you have to launch the server, ProxPy.

 ```bash 
 
Usage: ProxPy3.py [-h] [-p Port] [-d Debug] [-t Timeout] [-b BUFFER]
                  [-c MAX_CONN] [-fs FILTER_SERVER] [-fc FILTER_CLIENT]

Welcome to ProxPy's help page

optional arguments:
  -h, --help            show this help message and exit
  
  -p Port, --port Port  Provide an integer that will be our listen port
                        (default = 8080)
                        
  -d Debug, --debug Debug
                        Provide an integer that will be our debug level
                        
  -t Timeout, --timeout Timeout
                        Provide an integer that will be ProxPy activity
                        timeout
                        
  -b BUFFER, --buffer BUFFER
                        Provide an integer that will be our buffer size(Bytes)
                        
  -c MAX_CONN, --max_conn MAX_CONN
                        Provide an integer that will be max client conn
                        avaible with ProxPy
                        
  -fs FILTER_SERVER, --filter_server FILTER_SERVER
                        Provide an [url] to restrict access to that URL only
                        
  -fc FILTER_CLIENT, --filter_client FILTER_CLIENT
                        Provide an IP range that will be permitted to use
                        ProxPy


For more help you can check my github page: github.com/davidcawork

```

* Second, you must configure your web browser to connect it with the ProxPy. **Support only for Firefox**

* Third, run the log server.

```bash
python logger.py [Listen Port]
```
<br />

---- 
<br />

# Deployment of ProxPy in Amazon AWS

<br />
  
[![Watch the video](https://i.ibb.co/RHnkxVr/1.jpg)](https://www.youtube.com/watch?v=THR_xO13Gro)
<br />
  
