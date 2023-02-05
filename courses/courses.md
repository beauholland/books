
# 2023-02-02 ACloudGuru: Building Microsoft Azure Logic Apps
https://learn.acloud.guru/course/e493ba6c-795b-4ec8-8f23-b94310b3808e/overview
- ARM Templates
- Azure Portal "Deploy a custom template" to build your own template
- Azure DevOps: Azure Resource Manager Template Deployment
- Azure Log Analytics and Azure Monitor
  - In new Log Analytics: Overview > Configure monitoring solutions > "View Solutions" > Click "Add"
  - Search for "Logic App"
  - Find "Logic Apps Management (Preview)"
  - Click "Create"
  - Goto Logic App > Diagnostic settings > Add Diagnostic Settings
  - Send "Workflow runtime diagnostic setting" + "All Metrics" > send to log analytics workspace
  - Can take 30 minutes for new diagnostic settings to take effect
  - To view info in Log Analytics goto "Workspace Summary"
- Log Analytics Query example
```
Azure Diagnostics
| where ResourceProvider == 'MICROSOFT.LOGIC'
| where Category == 'WorkflowRunTime'
| where OperationName has 'workflowTriggerStarted' or OperationName has 'workflowActionStarted'

```
- VS Code "Logic App" extension

# 2023-02-01: Udemy: GitHub Actions - The complete guide
https://pipefish.udemy.com/course/github-actions-the-complete-guide

## Something



# 2023-02-01: Udemy: Data Integration Guide 
https://pipefish.udemy.com/course/data-integration-guide

## Main Features
- Integrate disparate systems
- Provide Connectivity Layer via Connectors
- Provide Business Process Layers via Orchestration
- Provide Common integration services: Error and exception handling, logging, notifications and reporting
- Support Service Composition and modular architecture
- Provide data transformation features

## Data Integration Patterns
- Point to Point
  - Directly connecting
  - N-1 issue
- Extract Tranform Load (ETL)
  - Suitable for bulk
  - Heavy, can impact performance
  - Latency, not suitable for real-time or on-demand
  - Heavily depdenant on databases, any schema changes could break
  - Best practices
    - Data movement should be done in delta mode
    - Queries on source and target database are optimized: indexes etc
    - Performance testing plan to anticipate during test phase
  - Variants and alternatives
    - Staging: eg for data cleansing, aggregate pre-calcs
    - Extract Load Transform: transformation is pushed towards target database after data is loaded "as-is"
    - Virtual ETL
- Enterprise ServiceBus and WebServices
- Electronic Data Interchange (EDI)
  - X12, EDIFACT

## Data Integration Projects
- Step 1: Ask the right questions
  - Identify your business contacts
    - Sponsors
    - Workshops
  - Identify and formalize the business use cases
    - Pain points
    - drivers
    - business domains
    - Risks
  - Identify how those problems are addressed today
    - Solutions already in place?
    - Any past initiatives and lessons learned?
- Step 2: Identify business use cases and value
  - Use Business Value (X axis) 1-5 : 5 = most value
  - Use Technical complexity (Y axis): 5 = easiest to solve
  - Use lead time (another axis)
- Step 3: Solution Panel
  - Assessment criteria: pricing, deployment options, performance
  - Table: Domain, Criteria, Weight, Option a,b,c
- Step 4: MVP
  - MVP success criteria
  - MVP governance
- Step 5: Industrialization plan
  - From Prototype to Maturity: more confidence
- Step 6: Solution & Project Methodology choices
  - Features: supported patterns (ETL), data transformation cap, connectors
  - Tech requirements: capacity, performance, error handling, logging, monitoring, automation, deployment
  - Operational requirements: maintainability, support, partner network
  - Agile, Scrum
- Step 7: Project Execution
  - Governance, Steering committees, communication, cut-over plan, go-live
- Step 8: Transition to Run

## Operations Management
- Sofware Vendor Support
- Monitoring and Alerts
- Incidents Management
  - SLAs, KPIs
- Environment Management
  - Pre-prod, Prod
  - user onboarding, offboarding
  - archiving

## Licensing and pricing
- Perpectual (CAPEX) vs Subscription (OPEX)
- Support Levels
- TCO: estimate your total cost of ownership: license, support, hosting, labor


