# WhatNext Vision Motors: Shaping the Future of Mobility with Innovation and Excellence
## Use Case
WhatsNext Vision Motors is revolutionizing its customer experience and operational efficiency with a cutting-edge Salesforce CRM implementation. The project streamlines the vehicle ordering process by auto-assigning orders to the nearest dealer based on customer location and preventing orders for out-of-stock vehicles. Automated workflows update order statuses dynamically and send scheduled email reminders for test drives. Key technical implementations include Apex triggers for stock validation, batch jobs for stock updates, and scheduled Apex for automated order processing. This initiative enhances customer satisfaction, improves order accuracy, and boosts overall operational efficiency.

## STEPS
### 1. Create Custom Object
A custom object is created to store vehicle order records, enabling WhatsNext Vision Motors to manage customer requests, dealer assignments, and stock validation within Salesforce. This object serves as the core data structure for the entire ordering process.
<img width="1916" height="554" alt="image" src="https://github.com/user-attachments/assets/15e4bd00-04ce-4eec-a89e-fe235d54e43d" />

### 2. Create Tabs
Custom tabs are added to make the new objects easily accessible from the Salesforce UI.
<img width="1919" height="593" alt="image" src="https://github.com/user-attachments/assets/f328f96b-7005-4250-9f07-26f576d99a55" />

### 3. Create Lightning App
A dedicated Lightning App is built to centralize all related objects, tabs, and tools in one workspace. This improves usability and ensures that all order management functionality is easily accessible to operational teams.
<img width="1918" height="722" alt="image" src="https://github.com/user-attachments/assets/30788655-9067-4417-8e7a-4df05a692cdb" />

### 4. Create Field and Relationship Field
Custom fields and lookup relationships are configured to link vehicle orders with customers, vehicles, and dealers. These fields support the logic used for stock validation, dealer assignment, and order status updates.
one of the example
<img width="1916" height="843" alt="image" src="https://github.com/user-attachments/assets/e7c6511c-1522-42de-9e70-936e67f4df84" />

### 5. Build A Flow
- Auto Assign Dealer: Automatically assigns the nearest dealer to a customer’s order based on their address, improving order accuracy and reducing manual effort.
<img width="1911" height="993" alt="image" src="https://github.com/user-attachments/assets/4fbf68f4-f9d1-4758-a9db-1fa526ae32a2" />

- Test Driver Reminder: Sends automated reminders to customers scheduled for a test drive, enhancing customer engagement and service continuity.
<img width="1918" height="993" alt="image" src="https://github.com/user-attachments/assets/83b9bacd-a869-48a2-878b-8426c3dab906" />

### 6. Create Apex and Trigger Batch Jobs
- Vehicle Order Trigger Handler and Vehicle Order Trigger: Validates vehicle stock and prevents order creation when items are unavailable.
- Vehicle Order Batch: Processes bulk updates to order status based on real-time stock availability.
- Vehicle Order Batch Scheduler: Runs the batch job at set intervals to keep all pending and confirmed orders up-to-date automatically.

## Conslusion
This Salesforce implementation significantly enhances the operational efficiency and customer experience at WhatsNext Vision Motors. Automated dealer assignment, real-time stock verification, and scheduled order updates reduce manual workload and ensure high accuracy. By combining Flows, Apex logic, and scheduled processes, the system provides a seamless ordering journey that supports faster processing, improved communication, and higher customer satisfaction.
