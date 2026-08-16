\# BPMN Process Explanations



\## Scenario 1: Employee Leave Approval



\### Objective



Model the process followed when an employee submits a leave request through the company's HR system.



\### Process Flow



1\. The process starts when the employee submits a leave request.

2\. The HR system checks the employee's leave balance.

3\. An exclusive gateway checks whether sufficient leave balance is available.

4\. If the balance is insufficient, the system sends an insufficient-balance notification and the process ends.

5\. If sufficient balance is available, the request is sent to the manager for approval.

6\. The manager's decision is handled through another exclusive gateway.

7\. If the manager rejects the request, the system sends a rejection notification and the process ends.

8\. If the manager approves the request, the system updates the employee's leave balance.

9\. The system sends an approval notification.

10\. The process ends.



\### BPMN Elements



\- Start Event

\- Tasks

\- Exclusive Gateways

\- Sequence Flows

\- End Events



\---



\## Scenario 2: Online Purchase Order Processing



\### Objective



Model the process used to handle an online customer purchase order.



\### Process Flow



1\. The process starts when a customer places an order.

2\. The system checks product availability.

3\. An exclusive gateway determines whether the product is available.

4\. If the product is unavailable, the system notifies the customer that the product is out of stock and the process ends.

5\. If the product is available, the system processes the payment.

6\. A second exclusive gateway determines whether the payment was successful.

7\. If payment fails, the system notifies the customer about the payment failure and the process ends.

8\. If payment succeeds, the system confirms the order.

9\. The product is prepared for shipment.

10\. The order is shipped.

11\. The customer receives a shipping confirmation.

12\. The process ends.



\### BPMN Elements



\- Start Event

\- Tasks

\- Exclusive Gateways

\- Sequence Flows

\- Multiple Process Paths

\- End Events



\---



\## Scenario 3: IT Service Request



\### Objective



Model the process used to handle an employee IT support request.



\### Process Flow



1\. The process starts when an employee reports an IT problem.

2\. The employee submits an IT support request.

3\. The help desk registers the request.

4\. The help desk checks the severity of the problem.

5\. An exclusive gateway determines the severity.

6\. A low-severity problem is assigned to a support technician.

7\. A high-severity problem is assigned to a senior technician.

8\. The technician investigates the problem.

9\. Another exclusive gateway checks whether the problem can be resolved internally.

10\. If it can be resolved internally, the technician fixes the problem.

11\. If it cannot be resolved internally, the problem is escalated to an external service provider.

12\. After resolution, the help desk updates the request status.

13\. The employee receives a resolution notification.

14\. The process ends.



\### BPMN Elements



\- Start Event

\- Tasks

\- Exclusive Gateways

\- Alternative Paths

\- Sequence Flows

\- End Event

