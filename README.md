# Local HTTPS Server  

This is a simple HTTPS server using Python's built-in `http.server` module with SSL encryption.  

## Requirements  

- Python 3.x  
- SSL certificate and key files (`server.crt` and `server.key`)  

## Generating Self-Signed Certificates  

If you haven't generated the required certificate files, create them using OpenSSL:  

```sh
openssl req -x509 -newkey rsa:2048 -keyout server.key -out server.crt -days 365 -nodes
