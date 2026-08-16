\# BPMN Process Modeling Assignment



\## Overview



This repository contains BPMN process models created for the BPMN process modeling assignment using Camunda.



The assignment consists of three business process scenarios:



1\. Employee Leave Approval

2\. Online Purchase Order Processing

3\. IT Service Request



\## Tool Used



\- Camunda Desktop Modeler

\- BPMN 2.0

\- OpenJDK 23



\## Project Structure



```text

bpmn-camunda-assignment/

│

├── README.md

│

├── models/

│   ├── scenario\_1\_employee\_leave\_approval.bpmn

│   ├── scenario\_2\_online\_purchase\_order\_processing.bpmn

│   └── scenario\_3\_IT\_service\_request.bpmn

│

├── documentation/

│   └── process-explanations.md

│

└── screenshots/

&#x20;   ├── scenario\_1\_employee\_leave\_approval.png

&#x20;   ├── scenario\_2\_online\_purchase\_order\_processing.png

&#x20;   └── scenario\_3\_IT\_service\_request.png


BPMN Scenarios

Scenario 1: Employee Leave Approval



This process models how an employee submits a leave request through the HR system.



The system first checks the employee's leave balance. If there is insufficient balance, an insufficient-balance notification is sent and the process ends.



If sufficient balance is available, the request is sent to the manager for approval. The manager can either approve or reject the request.



Approved request → leave balance is updated → approval notification is sent

Rejected request → rejection notification is sent

Insufficient balance → insufficient-balance notification is sent

Scenario 2: Online Purchase Order Processing



This process models the processing of an online customer order.



The system first checks whether the product is available. If the product is unavailable, the customer is notified and the process ends.



If the product is available, payment is processed. If payment fails, the customer is notified and the process ends.



If payment is successful, the order is confirmed, the product is prepared, the order is shipped, and the customer receives a shipping confirmation.



Scenario 3: IT Service Request



This process models the handling of an employee IT support request.



The help desk registers the request and checks the severity of the problem.



Low severity → assigned to a support technician

High severity → assigned to a senior technician



The technician then investigates the problem.



If the problem can be resolved internally, it is fixed. If it cannot be resolved internally, it is escalated to an external service provider.



After resolution, the request status is updated and the employee receives a resolution notification.



BPMN Elements Used



The models use basic BPMN building blocks including:



Start Events

Tasks

Exclusive Gateways

Sequence Flows

End Events

