# Web-Service-Composition-Server
Τhis is the API of the Web-Service-Composition Server created as part of the EU-funded project [S-CASE](http://www.scasefp7.eu/).
This page serves as usage instructions for the RESTful Web-Service-Composition web service.

## Media Types
This API accepts multipart POST and GET requests, while responses are in plain text.

## Error States
The common HTTP Response Status Codes are used.

## Check if a .war file already exists [/{fileName}]
This is the end point for checking if a .war file exists on server. It is a GET request with one URI parameter:
### fileName
String fileName: It is the name of the war file (including its extention).

The response is "text/plain" and it could be "true" or "false".

## Upload web service [/upload]
This is the end point for uploading the .war file of a web service in order to be deployed on server. The request is a MultiPart POST.
The response is "text/plain". An example of the response:

"File uploaded to : /home/ubuntu/apache-tomcat-8.0.30/webapps/Test-0.0.1-SNAPSHOT.war"

