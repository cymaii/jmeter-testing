# JMeter Performance Testing

## Website Tested
https://vnexpress.net

## Tool
Apache JMeter

## Thread Group 1
Users: 10  
Loop Count: 5  
Request: GET Homepage

## Thread Group 2
Users: 50  
Ramp-up: 30s  
Request: GET Homepage + Article page

## Thread Group 3
Users: 20  
Duration: 60s  
Request: GET 2 sub pages

## Result
Website works normally under light load but response time increases under heavy load.
