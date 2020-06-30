# SImple_app_VGS

# Description:

A simple web application that sends the information entered on the page (card num, exp date, cvv) to the VGS vault and showing the secured tokens. The tokens can be used to reveal and show the original information.
VGS integration includes:
-	Inbound route to encrypt 3 fields (card num, exp date, cvv)
-	Outbound route to reveal the encrypted 3 fields and send clean data to the echo server (https://echo.apps.verygood.systems). 

# Installation:

- The most recent Python version is recommended to use with the application

- The application is using Flask framework. The installation process on different environments is described in the following guide:
https://flask.palletsprojects.com/en/1.1.x/installation/
- In order to use your local web application you can connect it to the ngrok cloud service which accepts traffic on a public address and relays that traffic through to the ngrok     process running on your machine and then on to the local address you specified.
  More information regarding using ngrok can be seen here: https://ngrok.com/docs

- To work with forward proxy via TLS, you need to use a certificate. Specify the full path to the cert file in the app/ routes.py 
  verify='/full/path/to/cert.pem'
  
# Usage:

After installation run the simple_app.py file.  The server should run locally. Use ngrok in order to expose a web server running on your local machine to the internet. 

# Roadmap:

-	Add verification to the data forms.
-	Add styles for better representation.
 


