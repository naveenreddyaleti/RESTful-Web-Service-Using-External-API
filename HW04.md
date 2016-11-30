# WEB-SERVICE-USING-EXTERNAL-API
#### TIME CONVERTER ####
* This web service converts time from four American time zones namely Eastern standard time, Central standard time, Pacific standard time, Mountain standard time to Indian standard time. There are two input fields, one is the selection drop-down for American time zone and the other is a time input which takes American time. The web services for this web app are accessible at /api/time?AmericanZone=EST&IST=HH:MM. This app takes the input values as get parameters and returns JSON-formatted dictionary result which indicates the time in Indian standard time.. I am accessing this  API service at        
http://ec2-52-37-54-12.us-west-2.compute.amazonaws.com/api/time?AmericanZone=PST&IST=HH:MM

Below is the request for converting the time.

##### API call #####
http://ec2-52-37-54-12.us-west-2.compute.amazonaws.com/api/time?AmericanZone=EST&IST=HH:MM

##### Parameters #####
1. AmericanZone='EST'or'CST'or'MST'or'PST' &  2. IST = HH:MM 

##### Process Description #####
When a query is made using URL:http://ec2-52-37-54-12.us-west-2.compute.amazonaws.com/api/time?AmericanZone=PST&IST=HH:MM, it will be routed
to the URL:http://ec2-174-129-87-87.compute-1.amazonaws.com/api/time?AmericanZone=PST&IST=HH:MM by our application and json data will be
returned. This json data will be captured and displayed back in the browser by our application.

##### Example of API call #####
```API
http://ec2-52-37-54-12.us-west-2.compute.amazonaws.com/api/time?AmericanZone=EST&IST=06:30
```

##### API Response #####
Response from server with header information
```Result
Request URL:http://ec2-52-37-54-12.us-west-2.compute.amazonaws.com/api/time?AmericanZone=EST&IST=06:30
Request Method:GET
Status Code:200 OK
Remote Address:52.37.54.12:80
Content-Length:19
Content-Type:application/json
Date:Wed, 30 Nov 2016 04:14:09 GMT
Server:Werkzeug/0.11.11 Python/2.7.12

From the above it is clear that server response is in the form of json data type
