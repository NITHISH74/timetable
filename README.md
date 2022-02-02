# Experiment_Time_Table

## AIM
To Write a html webpage page to display your timetable.

# ALGORITHM
### STEP 1
create a simple table using table tag.
### STEP 2
Add header row using th tag.
### STEP 3
Add your timetable.
### STEP 4
Execute the program.

# CODE
```
from http.server import HTTPServer, BaseHTTPRequestHandler
content = """
<!DOCTYPE html>
<html>
<center>
   <head>
    <title>TIME TABLE</title>
  </head>
   <body>
      <table border = "1" cellspacing="1" bordercolor="#C19A6B" bgcolor="transparent">
         <tr>
            <th colspan="8">TIME TABLE</th>
            <br></br>
	 <table border = "1" cellspacing="1" bordercolor="#C19A6B" bgcolor="transparent">
    <br></br>
    <img src="https://cdn.discordapp.com/attachments/533340656987275284/914068516334891028/logo.png" width="662" height="100">
 <tr>
 <th colspan="8">TIME TABLE</th>
 </tr>
 <tr>
  <br></br>
<th colspan="4">NAME: NITHISHWAR S</th> 
<th colspan="4">REFERENCE NUMBER: 21002766 </th> 
         </tr>
         
         <tr>
            <th>DAYS</th>
            <th>1</th>
            <th>2</th>
            <th>3</th>
            <th>4</th>
                        <th rowspan="5">lunch break</th>

            <th>5</th>
                                   

            <th>6</th>
         </tr>
          <tr>
             <td align="center">MONDAY</td>
             <td align="center">19AI401/Obed Otto C</td>
             <td align="center">19AI401/Obed Otto C</td>
             <td align="center">19MA221/Archana SH</td>
             <td align="center">19MA221/Archana SH</td>
             <td align="center">19MA220/Archana SH</td>
             <td align="center">19MA220/Archana SH</td>
         </tr>
	 <tr>
             <td align="center">TUESDAY</td>
             <td align="center">----</td>
             <td align="center">----</td>      
             <td align="center">19AI302/Sridhar S</td>
             <td align="center">19AI302/Sridhar S</td>
             <td align="center">19AI302/Sridhar S</td>
             <td align="center">19AI302/Sridhar S</td>
         </tr>
	 <tr>
             <td align="center">WEDESDAY</td>
             <td align="center">----</td>
             <td align="center">----</td>
             <td align="center">19AI301/Archana SH</td>
             <td align="center">19AI301/Archana SH</td>
             <td align="center">19AI401/Obed Otto C</td>
             <td align="center">19AI401/Obed Otto C</td>
         </tr>
	 <tr>
             <td align="center">THURSDAY</td>
             <td align="center">19AI303/Sridhar S</td>
             <td align="center">19AI303/Sridhar S</td>
             <td align="center">19MA301/Archana SH</td>
             <td align="center">19MA301/Archana SH</td>
             <td align="center">19AI303/Sridhar S</td>
             <td align="center">19AI303/Sridhar S</td>
         </tr>
  	 <tr>
             <td align="center">FRIDAY</td>
             <td align="center">----</td>
             <td align="center">----</td>
             <td align="center">19MA301/Archana SH</td>
             <td align="center">19MA301/Archana SH</td>
             <td align="center">Mentoring/ECA051-AD/Niha K</td>
             <td align="center">19AI401/Obed Otto C</td>          
             <td align="center">19AI401/Obed Otto C</td>
             
         </tr>
         
      </table>
      <h2><b>Enrolled Subject</b></h2>
<H3>1. 19AI301 - Python Programming</H3>
<H3>2. 19AI302 - Engineering Design and Modelling</H3>
<H3>3. 19AI303 - Engineeering Mechanics and Product Development</H3>
<H3>4. 19AI401 - Fundamentals of Web Technology</H3>
<H3>5. 19MA220 - Mathematics for Artificial Intelligence</H3>
<H3>6. 19MA221 - Linear Algebra Laboratory</H3>
    
<center><br><br><div class="footer">

      
   </body>

</body>
  
</html>
"""
class myhandler(BaseHTTPRequestHandler):
    def do_GET(self):
        print("request received")
        self.send_response(200)
        self.send_header('content-type', 'text/html; charset=utf-8')
        self.end_headers()
        self.wfile.write(content.encode())
server_address = ('',8080)
httpd = HTTPServer(server_address,myhandler)
print("my webserver is running")
httpd.serve_forever()
```

# OUPUT
![image](https://user-images.githubusercontent.com/94164665/144058615-b37433c2-ea7a-4d7b-afb8-03cd9b3bbd7f.png)
![image](https://user-images.githubusercontent.com/94164665/144058641-73ae1a0b-a487-48a2-88b5-d298c2475731.png)
![image](https://user-images.githubusercontent.com/94164665/144059646-26de6992-ed95-4218-8934-cc3ef2ced6a4.png)


# RESULT
The above program is shown my time table successfully.
