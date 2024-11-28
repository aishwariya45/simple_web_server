# EX01 Developing a Simple Webserver

<<<<<<< HEAD
# Date:27/11/2024
=======
# Date: 27/11/2024
>>>>>>> f6afd37ba788784df3fbd38e95ecfe9db68dcfc3
# AIM:
To develop a simple webserver to serve html pages and display the configuration details of laptop.

# DESIGN STEPS:
## Step 1:
HTML content creation.

## Step 2:
Design of webserver workflow.

## Step 3:
Implementation using Python code.

## Step 4:
Serving the HTML pages.

## Step 5:
Testing the webserver.

# PROGRAM:
```
from http.server import HTTPServer, BaseHTTPRequestHandler
content = """
 <!doctype html>
 <html>
    <CENTER>
    <body bgcolor="PURPLE">
        <table border="5" cellpadding="22" aling="center" bgcolor="cyan">
            <h1><caption align="center">LAPTOP CONFIGURATION </caption></h1>
            <h3><caption align="center"><b>AISHWARIYA S 24900840</b></caption></h3>
        
        <tr bgcolor="blue">
            <th>S.NO</th><th>SYSTEM CONFIGURATION</th><th>DESCRIPTION</th>
        </tr>e
        <tr>
            <th>1</th><th>PROCESSOR</th><th>i5</th>
        </tr>
        <tr>
            <th>2</th><th>PRIMARY MEMORY</th><th>RAM 16GB</th>
        </tr>
        <TR>
            <th>3</th><th>SECONDARY MEMORY</th><th>512 GB</th>
        </TR>
        <tr>
        <th>4</th><th>OS</th><th>WINDOWS 11</th>
        </tr>
        <tr>
        <th>5</th><th>GRAPIC CARD</th><TH>NVIDIA</TH>
        </tr>
        </table>
 </body>
</CENTER>
 </html>
"""
class myhandler(BaseHTTPRequestHandler):
  def  do_GET(self):
     print("request received")
     self.send_response(200)
     self.send_header('content-type', 'text/html; charset=utf-8')
     self.end_headers()
     self.wfile.write(content.encode())
server_address = ('',8000)
httpd = HTTPServer(server_address,myhandler)
print("my webserver is running...")
httpd.serve_forever()
```
# OUTPUT:
<<<<<<< HEAD
![alt text](<Screenshot 2024-11-28 090507.png>)
=======
![Screenshot 2024-11-27 164512](https://github.com/user-attachments/assets/bb6848a3-d82f-49b1-bac9-62452ed1a55d)

![Screenshot 2024-11-27 163304](https://github.com/user-attachments/assets/330518e5-4835-4da7-b540-6bb0e0121157)

>>>>>>> f6afd37ba788784df3fbd38e95ecfe9db68dcfc3

![alt text](<Screenshot 2024-11-28 090435.png>)
# RESULT:
The program for implementing simple webserver is executed successfully.
