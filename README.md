# Ravin-Academy
🧠 Smart Management System – Functional Description

This application is designed to manage and track tasks, training, and performance across multiple roles within the organization. It includes four primary modules:

⸻

📌 1. Task Management for Area Managers and Store Managers
	•	The Admin or an Area Manager can create a task (e.g. “Stock Receiving”).
	•	Once a task is created, it will automatically be assigned to all store managers under that Area Manager.
	•	Each store manager will:
	•	See the task individually.
	•	Update the task status (e.g. Not Started, In Progress, Completed).
	•	Add notes if needed.
	•	The system should display analytics to the task creator showing:
	•	Who responded.
	•	Who didn’t respond.
	•	Task completion status across the entire group.

🔁 Tasks are distributed based on hierarchy: Each manager sees only what is assigned to them via their Area Manager.

⸻

🎓 2. Employee Training Tracker
	•	Each employee has a personal account.
	•	They receive individual training videos or content (e.g. “Customer Service Video”, “How to use the Cashier”).
	•	The system tracks:
	•	Training title
	•	Assigned by whom
	•	Training status (Not Started, In Progress, Completed)
	•	Notes or feedback from the employee

📥 Employees only see training assigned to them, not global training content.

⸻

🎯 3. Manager Training Module
	•	Area Managers and Store Managers also receive training materials tailored for their roles.
	•	Each manager will:
	•	Receive specific training video links.
	•	Mark the training as complete or in progress.
	•	Add any notes if needed.

The same logic as the employee training tracker applies here, but for management-level content.

⸻

📊 4. Sales Dashboard Module
	•	A live dashboard is connected to Google Sheets and shows performance insights for each store.
	•	Data includes:
	•	Branch name
	•	Sales Target vs. Actual Sales
	•	Target achievement percentage
	•	Best performing branch
	•	Lowest performing branch
	•	Average number of items per invoice
	•	Average invoice value

All this data can be viewed by Admins and Area Managers for tracking and decision-making.

⸻

🔐 Login & Permissions System
	•	Each user logs in using their email address.
	•	A User Role system is in place:
	•	Admin
	•	AreaManager
	•	Manager
	•	Employee
	•	Using role-based visibility, users will:
	•	Only see what is related to them.
	•	Not access other users’ data or tasks.

⸻

✅ Technical Summary
	•	The app is built with Glide using Google Sheets as the backend.
	•	Key Sheets:
	•	Users → Stores emails and roles.
	•	Managers → Links managers to their Area Managers.
	•	Employees → Links employees to their direct managers.
	•	ManagerTasks → Tasks assigned by Admins or Area Managers.
	•	ManagerTaskStatus → Responses from each manager to assigned tasks.
	•	EmployeeTraining → Individual employee training tasks and tracking.
	•	ManagerTraining → Individual manager training tasks and tracking.
	•	SalesDashboard → Sales and performance data for each store.
