DatabaseProblems Bug log xxu46
How to find the problem src in JavaEE project,

look at the console and find the first file that your team write(not from the library)

================

Eclipse Online Book Sales System
Bug1: 404 page not for register.jsp
<br>
Reason:
<br>
   url not match, use client/register.jsp rather than register.jsp
<br>
fix:
<br>
  change the url in the RegisterUIServlet
  
<br><br><br>
Bug2: sql exception, column does not match
reason:
cellphone and phone in the database
fix:
  changeh the database schema and fix it
  
  
login succuess
Bug3: created order failed
reason:
    Data truncation: Incorrect datetime value: '06-24-2014' for column 'ordertime' at row 1 Query: insert into orders(id,ordertime, price,state,user_id) values(?,?,?,?,?) Parameters: [32ca391b-45b5-408d-88a7-ff5b1a8b1786, 06-24-2014, 54.0, false, f60146ad-4b8c-4d8d-8f4f-6ce26f597d52]
 
how to fixed:
     I change the datetime to string, convert datetime to string

