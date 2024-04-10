# Bahceden
Bahceden is an innovative e-commerce Android application that eliminates intermediaries between local producers and customers. We aim to create a transparent and fair marketplace that empowers local producers and gives customers access to healthier, more affordable products.

## Summary
Bahceden offers a platform for local producers to sell their goods directly to consumers, cutting out middlemen who often exploit the system by buying products at low prices and selling them at inflated rates. We provide an intelligent price prediction system and up-to-date market data to assist both parties, enabling producers to make informed pricing decisions.

## Technologies Used
- Android Studio: This is for front-end development and intuitive user interface creation.
- Retrofit: To simplify network communication and handle HTTP requests between frontend and backend.
- Firebase: Integrated for authentication services, including sign-in and sign-up features.
- Spring Framework: Used to build a REST API for seamless communication between frontend and backend.
- Lombok: Java library that reduces repetitive code in the backend and improves development efficiency.
- MySQL: Chosen as the database management system to store crucial data for the app.
- Jsoup and Selenium: Libraries utilized for web scraping to gather and organize data from online sources.
- 
## Screenshots

| App Overview |
|:------------:|
| ![App Overview](/screenshots/overview.png) |
| *Provides an overview of the Bahceden app, showcasing the technologies used and their relationships.* | 

| Class Diagram |
|:-------:|
| ![Class Diagram](/screenshots/class_diagram.png) |
|*The class diagram illustrates the Java classes implemented in the app, along with their members and functions.* |

| Sitemap |
|:-------:|
| ![Sitemap](/screenshots/sitemap.png) |
| *The sitemap displays the user interactions within the app, guiding users through each site.* |

| Database Schema |
|:---------------:|
| ![Database Schema](/screenshots/database.png) |
| *This image showcases the database schema implemented in the backend using MySQL.* |

| Choose User Type | Login | Signup |
|:----------------:|:-----:|:------:|
| ![Choose User Type](/screenshots/choose_type.png) | ![Login](/screenshots/login.png) | ![Signup](/screenshots/signup.png) |
| *Users select their user type (producer or customer) on the Choose User Type page.* | *The Login page facilitates user authentication, including options to login with Google or using email/password.* | *The Signup page allows new users to create accounts, providing similar authentication options.* |

| Forgot Password | Customer Main Page | Product Page |
|:---------------:|:------------------:|:------------:|
| ![Forgot Password](/screenshots/forgot_password.png) | ![Customer Main Page](/screenshots/customer_main.png) | ![Product Page](/screenshots/product.png) |
| *Users can reset their passwords using the Forgot Password page, utilizing email or phone number.* | *The Customer Main Page lists products available for purchase.* | *The Product Page displays detailed information and prices for each product.* |

| Producer Page | Cart Page | Checkout Page |
|:-------------:|:---------:|:-------------:|
| ![Producer Page](/screenshots/producer.png) | ![Cart Page](/screenshots/cart.png) | ![Checkout Page](/screenshots/checkout.png) |
| *The Producer Page shows information about producers, including their address, name, and description.* | *The Cart Page lists products added to the cart along with their quantities.* | *The Checkout Page allows users to pay and finalize their orders.* |

| Profile Page | Edit Profile Page | Add Product Page |
|:------------:|:------------------:|:----------------:|
| ![Profile Page](/screenshots/profile.png) | ![Edit Profile Page](/screenshots/edit_profile.png) | ![Add Product Page](/screenshots/add_product.png) |
| *The Profile Page displays user profiles, while the Edit Profile Page allows users to make changes to their profiles.* | *The Add Product Page enables producers to add new products for sale within the app.* | *Producers can edit product information using the Edit Product Page.* |
  
# Bahceden App Setup Guide
Welcome to the Bahceden application setup guide! This guide will walk you through setting up your local development environment.

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
You can just enter the username and password you set in your backend's 'application.properties' file.
Click 'Test Connection' to ensure everything is set up correctly.
If the connection is successful, click 'OK' to save the connection.
Once the connection is established, you can open the SQL scripts located in the 'res' folder and then go ahead and execute them in the order below. This will set up the necessary tables for your application.

createDB.sql > createUser.sql > createTable.sql

After successfully importing the project, navigate to the 'bahceden-backend\src\main\resourcesapplication.properties' file. Update the MySQL username and password as per your MySQL server setup.
spring.datasource.username=\<your-username>
spring.datasource.password=\<your-password>

#### 2. Spring Boot Backend Setup

Open the terminal in "bahceden-backend" and run the lines below in order.

```sh
./mvnw package 
./mvnw spring-boot:run 
```

#### 3. Android Frontend Setup
Clone the repository and open the project in Android Studio:
Once you have the project open, you can run the Android application on your device or emulator.
