# Bahceden

Bahceden is an innovative e-commerce Android application that eliminates intermediaries between local producers and customers. Our goal is to create a transparent and fair marketplace that empowers local producers and provides customers with access to healthier and more affordable products.

## Summary

Bahceden offers a platform for local producers to sell their goods directly to consumers, cutting out middlemen who often exploit the system by buying products at low prices and selling them at inflated rates. To assist both parties, we provide an intelligent price prediction system and up-to-date market data, enabling producers to make informed pricing decisions.

## Technologies Used

- Android Studio: For frontend development and creating an intuitive user interface.
- Retrofit: To simplify network communication and handle HTTP requests between frontend and backend.
- Firebase: Integrated for authentication services, including sign-in and sign-up features.
- Spring Framework: Used to build a REST API for seamless communication between frontend and backend.
- Lombok: Java library that reduces repetitive code in the backend and improves development efficiency.
- MySQL: Chosen as the database management system to store crucial data for the app.
- Jsoup and Selenium: Libraries utilized for web scraping to gather and organize data from online sources.
  
# Bahceden App Setup Guide
Welcome to the Bahceden application setup guide! This guide will walk you through how to get your local development environment set up.

### Prerequisites
Before we begin, make sure you have the following tools installed on your system:

Android Studio
MySQL Workbench
MySQL Server
Java Development Kit (JDK)

### Steps to Set Up
#### 1. MySQL Database Setup
Launch MySQL Workbench and establish a new connection to your MySQL Server:

Click the '+' symbol next to 'MySQL Connections'.
Name your connection 'bahceden'.
Enter the username and password you set in your backend's 'application.properties' file.
Click 'Test Connection' to ensure everything is set up correctly.
If the connection is successful, click 'OK' to save the connection.
Once the connection is established, open the SQL scripts located in the 'res' folder and execute them in the order below. This will set up the necessary tables for your application.

createDB.sql > createUser.sql > createTable.sql

After successfully importing the project, navigate to the 'bahceden-backend\src\main\resourcesapplication.properties' file. Update the MySQL username and password as per your MySQL server setup.
spring.datasource.username=\<your-username>
spring.datasource.password=\<your-password>

#### 2. Spring Boot Backend Setup

Open terminal in "bahceden-backend" and run the lines below in order.

```sh
./mvnw package 
./mvnw spring-boot:run 
```

#### 3. Android Frontend Setup
Clone the repository and open the project in Android Studio:
Once you have the project open, you should be able to run the Android application on your device or emulator.
