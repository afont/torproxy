 
# Tor Proxy 

To deploy the Tor Squid Proxy, just follow steps below:

## Environment preparation:
```sh
$ #Install vagrant, virtualbox and ansible if not installed yet.
$ git clone https://github.com/afont/torproxy
$ cd torproxy
$ vagrant up
```
```
> Once machine is booted up, configure your browser to use new Tor Proxy, with the following parameters:
```
proxy server: 192.168.20.20
proxy port: 3128
```
