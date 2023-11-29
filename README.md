# Ex-01-Simple-Web-Server
## NAME : KAMALESH R
## REF NO : 23001711

## AIM:
To develop a simple webserver to serve html pages.

## DESIGN STEPS:
### Step 1: 
HTML content creation.

### Step 2:
Design of webserver workflow.

### Step 3:
Implementation using Python code.

### Step 4:
Serving the HTML pages.

### Step 5:
Testing the webserver.

## PROGRAM:
``````
from http.server import HTTPServer, 
BaseHTTPRequestHandler
content = """
<!doctype html>
<html>
<head>
<title>Top Five </title>
</head>
<body>
<h1>Top Five Web Application Development Frameworks</h1>
<h3>1.Django</h3>
<h3>2.MEAN Stock</h3>
<h5>3.React</h5>
</body>
</html>

class HelloHandler (BaseHTTPRequestHandler):
     def do_GET (self):
        self.send_response(200)
        self.send_header('Content-type', 'text/html; charset=utf-8')
        self.end headers ()
        self.wfile.write(content.encode())
        
server_address = ('', 80)
httpd = HTTPServer (server_address, HelloHandler)
httpd.serve_forever()

``````
## OUTPUT:
![Screenshot 2023-11-28 212744](https://github.com/KAMALESHNITHYA/ODD2023-WT-Ex-01-Simple-Web-Server/assets/145743119/d3f7cefd-f65a-457c-9fd3-0432c47884fd)


## RESULT:
The program for implementing simple webserver is executed successfully.
