Contact Form Project Installation Guide

Welcome to the installation guide for the Contact Form project! This guide will walk you through the process of setting up a web application that allows users to easily submit their contact information and messages through a form. The project is built using PHP for backend processing and MySQL for efficient data storage.

Features

Here's a rundown of the key features that the Contact Form project offers:

-> An intuitive contact form that includes fields for the user's full name, phone number, email, subject, and message.

-> Secure storage of submitted data in a MySQL database for convenient retrieval and reference.

-> Automatic email notifications triggered for each form submission, ensuring that designated recipients stay informed.


Prerequisites

Before you begin the installation, make sure you have the following prerequisites in place:

-> A web server that supports PHP (e.g., Apache, Nginx).

-> A functional MySQL database server.


Installation Steps

Follow these steps to get the Contact Form project up and running:

Step 1: Clone the Repository

To start, clone the project repository into your web server's root directory using the following command:

git clone https://github.com/saicharanchintu/PHP_TASK.git

If you're using the Apache server, clone the repository into the htdocs folder.

Step 2: Start Web Server and Configure MySQL

Start your web server and ensure that your MySQL database server is up and running. Create a new database specifically for this project.

Step 3: Set Up Database Table

Execute the provided SQL query to establish the required table structure within your chosen database:

CREATE TABLE contact_form (
    id INT AUTO_INCREMENT PRIMARY KEY,
    full_name VARCHAR(255) NOT NULL,
    phone_number VARCHAR(20) NOT NULL,
    email VARCHAR(255) NOT NULL,
    subject VARCHAR(255) NOT NULL,
    message TEXT NOT NULL,
    ip_address VARCHAR(45) NOT NULL,
    timestamp TIMESTAMP NOT NULL
);
Step 4: Access the Application

Open your preferred web browser and navigate to http://localhost/folder_name_in_htdocs, replacing folder_name_in_htdocs with the appropriate name of the folder where you cloned the repository.

By following these steps, you will have successfully installed and configured the Contact Form project on your web server.

