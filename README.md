## **Note:** To view the project metadata, download and unzip the force-app zip file and open the folders for flows, objects, tabs, applications, classes etc under the default folder.

# HandsMen-Threads-Fashion
Elevating the Art of Sophistication in Men's Fashion!
HandsMen Threads, a dynamic organization in the fashion industry, is embarking on a Salesforce project designed to revolutionize their data management and enhance customer relations. The project involves building a robust data model tailored to store all pertinent business data, ensuring a seamless flow of information across the organization.

A key aspect of this project is the maintenance of data integrity directly from the user interface (UI). This feature will safeguard the accuracy and consistency of the data, which is crucial for informed decision-making and reliable business operations.The project will integrate several new processes into the business workflow to improve customer service and operational efficiency:

1. **Automated Order Confirmations:** Post-order confirmation, customers will receive an email update, fostering engagement and strengthening customer relations.
2. **Dynamic Loyalty Program:** Customer loyalty statuses will be updated based on purchase history, enabling personalized rewards and promoting repeat business.
3. **Proactive Stock Alerts:** When stock levels drop below five units, automatic emails will notify the warehouse team, ensuring timely restocking and preventing stockouts.
4. **Scheduled Bulk Order Updates:** Daily midnight, the system will process bulk orders, updating financial records and adjusting inventory, ensuring accurate stock levels for daily operations.

## Objects and Fields: (ERD)
<img width="1869" height="529" alt="image" src="https://github.com/user-attachments/assets/ba4c2495-0cd8-469f-bb51-a7dc0479efb5" />

## Flows (Automation Strategy)
1. **Order Confirmation Flow:**
When the "Status" field = "Confirmed" in HandsMen order object, it sends an email alert to the customer's registered email ID.
<img width="395" height="667" alt="image" src="https://github.com/user-attachments/assets/5d5490c5-7710-4d07-9c68-de52ef81d119" />

2. **Loyalty Status Update Flow:**
Updates the loyalty status of the HandsMen customer object to gold, silver or bronze based on their total purchases field every day triggered at 12am.
<img width="953" height="871" alt="image" src="https://github.com/user-attachments/assets/9a675884-71e2-4821-b62a-bcebbf63e4b9" />

3. **Stock Alert Flow:**
Triggered when "Stock" field < 5 in inventory object.
<img width="395" height="658" alt="image" src="https://github.com/user-attachments/assets/dc37525c-58da-4828-ab2a-46a5ce25f352" />
