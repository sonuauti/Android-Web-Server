# Android Web Server
Simple and Low footprint TCP/IP Web Server for Android in Java

This is standalone, multithreaded, almost or No dependancy ! http server in Java with example use in Android.

# How to use it in Android

1.  Copy TinyWebServer.java class from src dir to your android project package
2.  Call following from android service or process
    
         //call contructor with local ip, port , public html directory path
       TinyWebServer.startServer("localhost",9000, "/web/public_html");

# How to write custom api 

1.  Copy AppApis.java from src directory
2.  keep the package name same for AppApis.java like "appapis.queryfiles" 
3.  open AppApis.java and write your own mehtod/function inside AppApis.java 
    for example,
    
    public String myfirstapi(HashMap qparms){
      //todo - write your api logic here
      //qparms is collection of GET and POST parameters
    }
    
    you can access this api -> http://localhost/myfirstapi
    
    

# How to check demo
  Run the code and hit browser with http://localhost:9000/helloworld 
  > here port number is 9000 
  > localhost or your device ip address
  > helloworld is api method inside AppApis.java
  
  

    
