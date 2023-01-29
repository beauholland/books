Solution architecture is not just about a software solution. It covers all aspects of a system, which will be included but not limited to, system infrastructure, networking, security, compliance requirement, system operation, cost, and reliability.

A solution architect’s responsibilities
- Analyze Functional Requirements
- Define non-functional requirements
  - performance
  - security & compliance
  - Recoverability
  - Maintainability
  - Reliability
  - Availability
  - Scalability
  - Usability
- understand and engage stakeholders
- understand constraints
- Technology Selection
- Prototyping and Proof of Concept
- Solution Design and Delivery
- Solution Scaling and technology evangelist

Architecure Constraints
- Quality
- Time
- Scope
- Technology
- Risk
- Resource
- Compliance
- Cost

Benefits of Solution Architect
- Addressing the business needs and quality of delivery
- Selecting the best technology platform
- Addressing solution constraints and issues
- Helping in resource and cost management
- Managing solution delivery and project life cycle
- Addressing non-functional requirements: 
  - disaster recovery
  - security & compliance
  - high availability
  - scalability
  - performance
  - maintainability 

Attributes of Solution Architecture Design:
- Scalability and Elasticity
- High availability and resiliency
- Fault tolerance and redundancy
- Disaster recovery and business continuity
  - Recovery Time Objective (RTO) = how much downtime a business can sustain without any significant impact
  - Recovery Point Objective (RPO) = indicates how much data loss a business can resist
- Extensibility and reuseability
  - loosely coupled architecture
  - queue based architecture
- Usability and accessibility
- Portability and interoperability
- Operational excellence and maintainability
  -  design should include how the workload will be deployed, updated, and operated in the long run 
  -  It is essential to plan for logging, monitoring, and alerting to capture all incident and take quick actions for the best user experience. Apply automation wherever possible, whether deploying infrastructures or changing the application code to avoid human error
- Security and compliance
  - Authentication and Authorization
  - Web security
  - Network security
  - Infrastructure security
  - Data security 
- Cost optimization and budets

Principles of Solution Architecture Design:
- Scaling workload
- Building resilient architecture
- Design for performance
- Using replaceable resources
- Creating immutable infrastructure = Pets vs Cattle
  - Pets get unique names and special treatment. When something goes wrong its repaired with significant time, cost
  - Cattle get numbers not names and recieve no special treatment. When something goes wrong its replaced NOT repaired
- Canary testing
- Think loose coupling
- Think service not server
  - think of SOA while designing a solution
  - The clear advantage of services is that you have a smaller surface area of code to maintain and services are selfcontained. You can build them with no external dependencies. All prerequisites are included in the service, which enables loose coupling, scaling, and reduces the blast radius in case of failure
- Using the right storage for the right need
  - Durability requirement: How should data be stored to prevent data corruption?
  - Data availability: Which data storage system should be available to deliver data?
  - Latency requirement: How fast should the data be available?
  - Data throughput: What is the data read and write need?
  - Data size: What is the data storage requirement?
  - Data load: How many concurrent users need to be supported?
  - Data integrity: How to maintain the accuracy and consistency of data?
  - Data queries: What will be the nature of queries?
- Think data-driven design
- Overcoming constraints
  - MoSCoW
  - Mo (Must have)
  - S (Should have)
  - Co (Could have)
  - W (Won't have)
  - plan a minimum viable product (MVP)
- Adding security everywhere
  - Physical security of data center
  - Network security
  - Identity and Access Management (IAM) 
  - Data security in-transit
  - Data security at rest
  - Security monitoring
- Automating everything
  - Application testing
  - IT infrastructure
  - Logging, monitoring, and alerting
  - Deployment automation
  - Security automation


Cloud-native 
- is about speed and agility
- Not just about enabling the business capabilities but fundamentally transforming and accelerating implementations
- Cloud-native systems are designed to embrace rapid change, large scale, and resilience
- Purist definition includes: microservices, containers, kubernetes, continuous delivery, devops, agile, etc
- I see the term cloud-native as:
  - "solutions or apps that are explicitly designed for optimal effectiveness within a cloud environment"
- No large upfront design, but knowing enough to make sure we are heading in the correct direction without going into a dead-end.
- If we didn't know enough we would SPIKE and prototype something out


Cloud Migration strategy
- On premises app
  - Application Discovery
    - Retire or Retain
    - Lift & Shift
      - Relocate
      - Rehost
      - Replatform
    - Cloud native
      - Refactor
      - Repurchase

Steps for cloud migration
- Discover
- Analyze
- Plan
- Design
- Migrate
- Integrate
- Validate
- Operate
- Optimize


Solution Architecture Design Patterns
- Building an n-tier layered architecture
  - multitier architecture
  -  divide your product functions into multiple layers, such as presentation, business, database, and services, so that each layer can be implemented and scaled independently
- Creating multi-tenant SaaS-based architecture
  -  single instance of the software and supporting infrastructure serve multiple customers
  -  At the data access layer, each tenant will have data level isolation with one of the following methods:
     -  Database Level Isolation
     -  Table Level Isolation
     -  Row Level Isolation
-  Building stateless and stateful architecture designs
-  Understanding SOA
   -  SOAs take monolithic applications and spread some of those operations out into individual services that operate independently to each other. The goal of using an SOA is to loosen the coupling of your application's services
-  Building serverless architecture
-  Creating microservice architecture
-  Building queue-based architecture
-  Creating event-driven architecture
   -  Event-driven architecture can also be based on the publisher/subscriber model or the event stream model
   -  Event stream model
-  Building cache-based architecture
