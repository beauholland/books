# Integrate 2023
https://www.serverless360.com/integrate-2023/

# Summary
- New Features to keep an eye out for
  - GitHub CoPilot, we need to start using it
  - Azure Integration Space
  - APIM
    - Workspaces
    - API Center
    - Microsoft Defender for APIs

# Keynote: State of Microsoft integration
Integration Space
- No doco
- Only sharing thoughts
- single pain view of integration code, infrastructure, application and business processes
- decouples infrastructure from code and configuration
- deployment target for integration code - workflows, apis, messaging and config
- unified experience for managing configuation

First features = End to End integration application monitoring
- business centric grouping of integration components workflows, apis, functions
- holistic view of all components of application
- rules, alerts and thresholds are defined in the context of application, not a specific resource

Business Process Tracking
- map multiple workflows to a single business process
- developers use familiar tools like designer and token picker to create a definition of the process
- data is gathered automatically no need to insert tracking actions into worklfow
- business users can see and visualize every transaction

# Getting started with Azure Integration Services
- Market trends: Azure Integration services, Azure Logic Apps roles are on the increase
- ChatGPT can build logic apps
- Azure Integration Services, Gartner Leaders
- June 22 = Logic Apps Aviators Day

# What is new in the world of Azure API Management?
-  The journey to api-first development
   -  API discovery and reuse
   -  security and compliance at runtime
   -  api testing and design
   -  observability and analytical capabilities
   -  inter-operability with multiple protocols and standards
   -  governance and security
-  API Center
-  GitHub CoPilot support for Policies
-  GitHub CoPilot X = good 
-  Azure Load Testing for APIs
-  Microsoft Defender for APIs

# API management for microservices in a hybrid and multi-cloud world
- Policy Outbound set header name ="X-Upstream-url" = context.Request.Url.ToString()
- Random Load Balancer Policy

# API Security deep dive
- OWASP Top 10 API Security Threats: https://owasp.org/www-project-api-security/
- https://www.shodan.io/dashboard
- CIA Triad = Confidentiality, Integrity, and Availability
  - Practical Security Handbook - Surviving and Thriving in Azure AIS with the VIA Triad: https://ninocrudele.com/practical-security-handbook-surviving-and-thriving-in-azure-ais-with-the-cia-triad
  - Azure Resources CIA Decision Matrix

# Experiences releasing APIs to API Management
- Samuel Kastberg
- Exported Files:
  - Spec
  - Settings file
  - Parameters file
  - Sample pipeline
- API release resources included:
  - Settings File:
    - Named Values
    - Backends
    - Additional Infomration eg: contact information
    - Compare with RS Kits config file: https://github.com/Azure/azure-api-management-devops-resource-kit
  - Parameter Files
    - Environment Specific settings
  - Pipelines
    - Managed Templates


# Logic Apps standard - The developer experience
- Call custom .net code using new Logic app action using new Workspace features


# Landing safely with Azure Integration Services
- https://github.com/Azure/Integration-Services-Landing-Zone-Accelerator
- Includes: Design Considerations, Design Recommendations
