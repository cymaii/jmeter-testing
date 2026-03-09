# JMeter Performance Testing

## Website Tested
https://vnexpress.net

Tool used: Apache JMeter

---

# Thread Group 1 – Basic Test

Configuration:

- Users: 10
- Loop Count: 5
- Request: HTTP GET Homepage

Result:

![Thread1](Thread Group 1.png)

Analysis:

This test simulates a small number of users accessing the homepage simultaneously. 
The system handled all requests successfully with no errors. 
Response time remained relatively low, indicating stable performance under light load.

---

# Thread Group 2 – Heavy Load Test

Configuration:

- Users: 50
- Ramp-up Period: 30 seconds
- Requests:
  - Homepage
  - Article page

Result:

![Thread2](Thread Group 2.png)

Analysis:

This scenario simulates heavier traffic. 
With 50 concurrent users, the response time increased but the system continued to process requests successfully. 
No errors were recorded, indicating the system can handle higher load conditions.

---

# Thread Group 3 – Custom Test

Configuration:

- Users: 20
- Duration: 60 seconds
- Requests:
  - Article 1
  - Article 2

Result:

![Thread3](Thread G3.png)

Analysis:

During the 60-second test period, the system processed more than 200 requests. 
The average response time was around 5 seconds and the error rate remained 0%. 
This indicates stable performance under moderate load conditions.

---

# Metrics Collected

The following metrics were analyzed:

- Response Time
- Throughput
- Error Rate

These metrics help evaluate how well the system performs under different load conditions.

---

# Conclusion

Through performance testing using Apache JMeter, the website demonstrated stable performance across different load scenarios. 

Even with multiple concurrent users, the system processed requests successfully without errors, although response time increased under heavier load.
