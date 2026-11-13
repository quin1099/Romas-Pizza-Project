# Romas-Pizza-Project
Roma's Pizza Online Ordering & Delivery Scheduling System

BACS 350 – Group Project
Team Name: The ScrumBags

Project Overview

Roma's Pizza Online Ordering & Delivery Scheduling System is a responsive web application designed to make ordering pizza easier and more convenient for customers while helping restaurant staff manage incoming orders.

The application allows customers to browse the restaurant menu, customize pizzas, manage a shopping cart, choose pickup or delivery, schedule a requested fulfillment time, and submit orders online.

Restaurant staff will have access to an administrative dashboard where they can view incoming orders, review scheduled fulfillment times, and update order statuses.

The goal is to create a realistic full-stack application that provides a simple customer ordering experience and an organized restaurant order-management system.

Team Members
Name	Scrum Role
Eric Quintana	Product Owner
David Agbosse	Scrum Master
Cade Huggins	Developer
Simon Herz	Team Contributor
Project Objectives
Create an easy-to-use online pizza ordering experience.
Allow customers to browse menu categories and view item prices.
Support pizza customization, including sizes and toppings.
Provide shopping cart functionality with automatic subtotal calculations.
Allow customers to register and sign in.
Support both pickup and delivery orders.
Allow customers to schedule requested pickup or delivery times.
Provide order confirmation and status updates.
Give restaurant staff the ability to view and manage incoming orders.
Develop a responsive interface for desktop and mobile devices.
Main Features
Customer Features
Menu Browsing
Browse pizza, sides, and drink categories.
View item names, descriptions, and prices.
Pizza Customization
Select pizza sizes.
Add or remove toppings.
View updated prices based on selections.
Shopping Cart
Add menu items to the cart.
Update item quantities.
Remove unwanted items.
View the current order subtotal.
Customer Authentication
Create a customer account.
Sign in with existing credentials.
Associate orders with customer accounts.
Pickup and Delivery
Choose pickup or delivery at checkout.
Enter delivery information when applicable.
Select an available fulfillment time.
Order Confirmation and Tracking
Review order details before submission.
Receive a unique order identifier.
View the current order status.
Restaurant Staff Features
Access a protected staff dashboard.
View incoming customer orders.
Review order items and customizations.
View scheduled pickup and delivery times.
Update order statuses.

Proposed order statuses include:

Received
Preparing
Ready / Out for Delivery
Completed
Technology Stack

The project is designed around the MERN stack.

Technology	Purpose
MongoDB	Database for storing users, menu items, and orders
Express.js	Backend web framework and API development
React.js	Frontend user interface
Node.js	Server-side JavaScript runtime
GitHub	Version control and team collaboration

Additional libraries and tools may be incorporated as development progresses.

Proposed Project Structure
text
romas-pizza-ordering/
│
├── client/
│   ├── public/
│   └── src/
│       ├── components/
│       ├── pages/
│       ├── services/
│       └── App.jsx
│
├── server/
│   ├── config/
│   ├── models/
│   ├── routes/
│   ├── controllers/
│   ├── middleware/
│   └── server.js
│
├── docs/
│   └── project-documentation/
│
├── README.md
└── .gitignore


Note: This is the proposed directory structure. It will be updated to reflect the actual repository as development progresses.

Database Design

The application is expected to use MongoDB to store the following information:

Users

User ID
Name
Email
Password hash
Account role (Customer or Staff/Admin)

Menu Items

Item ID
Name
Description
Category
Base price
Available customization options

Orders

Order ID
Customer information
Selected menu items
Quantities and customizations
Order total
Fulfillment method
Delivery address (when applicable)
Scheduled fulfillment time
Order status
Customer Ordering Workflow

The primary customer workflow is:

Visit the home page and browse the menu.
Select a menu item.
Customize pizza size and toppings.
Add items to the shopping cart.
Review and edit the cart.
Sign in or create an account if necessary.
Choose pickup or delivery.
Select an available fulfillment time.
Review and submit the order.
Receive order confirmation and view order status.
Staff Workflow
Staff member signs in.
Opens the administrative order dashboard.
Reviews incoming orders.
Checks order details and scheduled fulfillment times.
Updates order statuses as orders are prepared and fulfilled.
Development Methodology

The ScrumBags team is following Agile development principles and using Scrum practices to organize project development.

The team uses a product backlog to prioritize development tasks and a Kanban board to monitor task progress.

Our workflow includes:

Sprint planning and task assignments.
Regular team communication and progress updates.
Backlog prioritization.
Code development and integration.
Feature testing and review.
Sprint retrospectives and process improvements.
Getting Started

The following instructions describe the intended local development setup once the application source code and configuration files are available.

Prerequisites
Node.js and npm
MongoDB or a MongoDB Atlas connection
Git
A code editor such as Visual Studio Code
Installation

Clone the repository:

bash
git clone YOUR_GITHUB_REPOSITORY_URL


Navigate into the project directory:

bash
cd romas-pizza-ordering


Install frontend dependencies:

bash
cd client
npm install


Install backend dependencies:

bash
cd ../server
npm install

Environment Variables

Create an environment configuration file in the server directory.

Example:

env
PORT=5000
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=your_secure_secret


Do not commit actual passwords, database credentials, or secret keys to GitHub.

Running the Application

Start the backend server:

bash
cd server
npm run dev


Start the frontend in a separate terminal:

bash
cd client
npm run dev


Note: These commands assume the corresponding package scripts have been configured. Actual setup instructions will be updated to match the implemented application.

Project Scope

The initial course version will focus on the primary ordering and order-management workflows.

Included functionality:

Menu browsing
Pizza customization
Shopping cart
Customer registration and authentication
Pickup and delivery selection
Order scheduling
Order submission
Order confirmation and status
Staff order management

Live payment processing is outside the initial required scope. Checkout may represent the payment step without integrating an actual payment provider.

Security and Quality Requirements

The team intends to follow these technical practices:

Passwords must be securely hashed rather than stored as plain text.
Administrative functionality must require authorization.
User input must be validated.
Submitted orders should persist in the database.
The interface should support desktop and mobile screen sizes.
Code should be organized into reusable and maintainable components.
Contribution Guidelines

Team members should follow these practices when contributing:

Coordinate tasks with the team before beginning major changes.
Pull the latest repository changes before starting development.
Use descriptive branch names for feature development.
Write clear and descriptive commit messages.
Test changes before submitting them.
Review changes before merging into the main branch.
Keep documentation updated when functionality changes.
Academic Project Information

Course: BACS 350
Project: Roma's Pizza Online Ordering & Delivery Scheduling System
Team: The ScrumBags
Project Deliverables: Project Proposal and Progress Report

This project is being developed as part of a university course to demonstrate full-stack web development, database integration, software project management, and Agile collaboration.

Team ScrumBags – BACS 350
