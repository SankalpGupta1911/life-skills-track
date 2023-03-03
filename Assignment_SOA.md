# Service-Oriented Architecture

## Introduction

Service-oriented architecture (SOA) is an architectural approach in which we use services from third-party service providers without reinventing it ourselves as parts of various components and integrate these components as per our requirement to serve a bigger purpose or provide a high level collaborated/integrated service. SOA allows users to combine a large number of facilities from existing services to form applications.
SOA imbibes few design principles like interoperability and loose coupling to provide means for integrating components into a coherent and decentralized system. 

### Some examples of SOA
* To build a website we need a payment gateway, products shipment service, and web hosting. So we integrate payment gateways like Razorpay or Paypal and use any 3rd party shipment services and get hosting from hosting service providers like Hostinger or Bluehost. Now we don’t need to make our own payment gateway or our own web hosting company to make the website. The idea is to use already built products and expand your business without reinventing everything.

* Any hotel getting cab services and food prepared through any outer service provider.

* Any Edtech utilising payment gateways like Razorpay or UPI for transactions and using financial platforms like Propelled for EMI facilitation.

### Components of SOA
![Image Logo](https://media.geeksforgeeks.org/wp-content/uploads/Screenshot-248.png)


### Few Important terms to understand SOA better:
**Service Orchestration**
Services might collect information and data retrieved from other services to complete the request of a given service consumer.

**Service Choreography**
An important interaction pattern in which the coordinated interaction of services happens without a single point of control. 

**ESB**
An enterprise service bus (ESB) is software that you can use when communicating with a system that has multiple services. It establishes communication between services and service consumers no matter what the technology. An ESB provides communication and transformation capabilities through a reusable service interface. The ESB is a centralized service that routes service requests to the appropriate service. It converts request into a format that is acceptable by the service’s underlying platform and programing language.




## Basic principles of Service Oriented Architecture

Some basic principles are common across all SOA implementations.

1. **Interoperability** 
Each service in SOA includes description documents that specify the functionality of the service and the related terms and conditions. Any client system can run a service, regardless of the underlying platform or programming language. For instance, business processes can use services written in both C# and Python. Since there are no direct interactions, changes in one service do not affect other components using the service.

2. **Loose coupling**
Loose coupling of services means that they should be designed as self-contained components having as little dependency as possible on external resources such as data models or information systems. They should also be stateless without retaining any information from past sessions or transactions. This way, if you modify a service, it won’t significantly impact the client applications and other services using the service.

3. **Composability** By using services as building blocks, complex operations can be implemented. Service orchestration and choreography help in composing services and achieving business goals.

4. **Abstraction**
The code logics or implementation details are unknown to the service consumers. They get the required information about what the service does and how to use it through service contracts and other service description documents.

5. **Granularity**
Services in SOA should have an appropriate size and scope, ideally packing one discrete
business function per service. Developers can then use multiple services to create a composite service for performing complex operations.


## Advantages/Benefits of Service oriented architecture

1. **Faster:**
Reuse services across different business processes saves time and costs. Assembling applications is faster than writing code and performing integrations from scratch.

2. **Ease of maintenance:**
It’s easier to create, update, and debug small services than large code blocks in monolithic applications.Service is maintained by a 3rd party and any change in that service will not affect your system.

3. **Greater adaptability:**
SOA is more adaptable to advances in technology. You can modernize your applications efficiently and cost effectively. For example, healthcare organizations can use the functionality of older electronic health record systems in newer cloud-based applications.

4. **Same directory structure:**
Services have the same directory structure so that consumers can access the service data from the same directory every time. If any service has changed its location then also directory remains same.

5. **Prevents the hassle of reinventing:**
The service consumers can use pre-build service and don’t have to rebuild every functionality from scratch. This increase the productivity. Now the service consumer can focus on its own website or software without worrying about external component integration.

6. **Scalable:**
If the user base increases, then the application can be easily scaled by attaching more servers. This will make service available all time to the users.

7. **Reliable:**
Services are usually smaller and simpler in comparison to the full-fledged application. So it is easier to debug and test the independent services as third party vendors are accountable for service failures, maintenance and reliability.

8. **Independent of other services:**
Services are independent of each other, so they can be used by multiple applications at the same time.

9. **Platform independence:**
Services communicate with other applications through common language which means it is independent of the platform on which application is running. Services can provide API in different languages e.g. PHP, JavaScript etc.


## Disadvantages of Service Oriented Architecture

1. **Increased overload**
In SOA, all inputs are checked/validated before they are passed on to the service. Using multiple services overloads the system with extra computation.

2. **High cost:**
SOA is expensive in terms of human resource, development, and technology.

3. **High bandwidth server:**
As some web services send and receive messages and information frequently so they easily reach to a point of a million requests per day. So it requires a high-speed server with a lot of data bandwidth to run a web service.


## Limitations in implementing service-oriented architecture

* **Limited scalability**
System scalability is significantly impacted when services share many resources and need to coordinate to perform their functionality. 

* **Increasing interdependencies**
Service-oriented architecture (SOA) systems can become more complex over time and develop several interdependencies between services. They can be hard to modify or debug if several services are calling each other in a loop. Shared resources, such as centralized databases, can also slow down the system.

* **Single point of failure**
For SOA implementations with an ESB, the ESB creates a single point of failure. It is a centralized service, which goes against the idea of decentralization. Clients and services cannot communicate with each other at all if the ESB goes down.


**References:**


* [Geeks for geeks](https://www.geeksforgeeks.org/service-oriented-architecture/)
* https://www.itrelease.com/2018/10/advantages-and-disadvantages-of-service-oriented-architecture-soa/
* https://aws.amazon.com/what-is/service-oriented-architecture/#:~:text=Service%2Doriented%20architecture%20(SOA),other%20across%20platforms%20and%20languages.
* https://www.youtube.com/watch?v=sN6ku58fGF4
* https://www.youtube.com/watch?v=_dFJOSR-aFs
