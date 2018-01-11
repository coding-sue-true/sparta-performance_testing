# sparta-performance_testing

## Main

This repo was created to introduce us to JMeter and how to execute different types of performance testing:
- Spike, Soak, Stress and Load

### What is performance testing?

> - It is  a type of non-functional testing.
> - Performance testing is testing that is performed, to determine how fast >some aspect of a system performs under a particular workload.
> - It can serve different purposes like it can demonstrate that the system meets performance criteria.
> - It can compare two systems to find which performs better. Or it can measure what part of the system or workload causes the system to perform badly.
> - This process can involve quantitative tests done in a lab, such as measuring the response time or the number of MIPS (millions of instructions per second) at which a system functions.
>
 __Why to do performance testing:__
- Improve user experience on sites and web apps
- Increase revenue generated from websites
- Gather metrics useful for tuning the system
- Identify bottlenecks such as database configuration
- Determine if a new release is ready for production
- Provide reporting to business stakeholders regarding performance against expectations

>http://istqbexamcertification.com/what-is-performance-testing-in-software/


## Steps

- Image 1
  - Set up a Test Plan (In this case, we gave it the name of 'Post_codes')
  - The 'Thread Group' is where we will define the number of users and for how long to simulate a scenario.
![JMeter](/images/jmeter1.png)


- Image 2
  - 'HTTP Request Defaults' - Define the main URL link from where we get the data back
![JMeter](/images/jmeter2.png)


- Image 3
  - 'HTTP Header Manager' -> where you define the content-type you're getting. In this case is 'application/json'
![JMeter](/images/jmeter3.png)

- Image 4
  - 'HTTP Request' -> Where you define the route you want to get. In this case I'm requesting POST postcodes
![JMeter](/images/jmeter4.png)

- Image 5
  - 'Response Assertion' -> You can give it some input to check if you have that input in your test, if you do it passes, if you don't it fails.
![JMeter](/images/jmeter5.png)

- Image 6
  - 'JSON Extractor' -> Here you can set up some variables and it also allows you to access certain info from your request
![JMeter](/images/jmeter6.png)

- Image 7
  - 'View Results Tree' -> Where you can see the results of your tests. After you set up the amount of users and time in the 'Thread Group' part, and all the routes you want to test, you just have to press play and check the results in here.
![JMeter](/images/jmeter7.png)

- Image 8
  - 'HTTP Request' -> just another example of HTTP Request, but this time using the variables that were set up in

![JMeter](/images/jmeter8.png)

## Resources
- https://www.blazemeter.com/blog/advanced-usage-json-path-extractor-jmeter
- http://jmeter.apache.org/
- http://istqbexamcertification.com/what-is-performance-testing-in-software/
