# Food Ordering System

A web-based food ordering system built with **Spring Boot**, **Spring Data JPA**, **Thymeleaf**, and **MySQL**. It allows users to browse a menu, add items to a cart, mark favorites, place orders, and includes an admin panel for managing menu items.

## Table of Contents
- [Features](#features)
- [Technologies](#technologies)
- [Setup and Installation](#setup-and-installation)
- [Usage](#usage)
- [Project Structure](#project-structure)
- [Screenshots](#screenshots)
- [Contributing](#contributing)
- [License](#license)

## Features
- **User Authentication**: Login for users and admins (currently basic authentication, planned upgrade to Spring Security).
- **Menu Management**: Browse food items, view details, and add to cart or favorites.
- **Cart Functionality**: Add/remove items and checkout to place orders.
- **Favorites**: Save favorite menu items for quick access.
- **Order Management**: View, edit, and delete orders with pagination.
- **Admin Panel**: Add new menu items with image upload.
- **Responsive UI**: Built with Thymeleaf, CSS, and Font Awesome for a user-friendly experience.

## Technologies
- **Backend**: Spring Boot 3.5.0, Spring Data JPA, MySQL
- **Frontend**: Thymeleaf, HTML, CSS, Font Awesome
- **Build Tool**: Maven
- **Java Version**: 17
- **Database**: MySQL
- **Other**: Commons FileUpload for image uploads

## Setup and Installation
### Prerequisites
- Java 17
- Maven
- MySQL
- Git

### Steps
1. **Clone the Repository**:
   ```bash
   git clone https://github.com/yourusername/FoodOrder.git
   cd FoodOrder

- **Configure MySQL**:
- Create a MySQL database (e.g., foodorder_db).
- **Update**  src/main/resources/application.properties with your database credentials:
     ```bash
      spring.datasource.url=jdbc:mysql://localhost:3306/foodorder_db
      spring.datasource.username=your_username
      spring.datasource.password=your_password
      spring.jpa.hibernate.ddl-auto=update
      spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL5Dialect
      spring.servlet.multipart.max-file-size=10MB
      spring.servlet.multipart.max-request-size=10MB
- **Build the Project**: mvn clean install
- **Access the application at**
   ```bash
      http://localhost:8080.

- **Usage**
- Home Page: Browse the menu, add items to cart or favorites.
- Login: Access user-specific features like cart and orders.
- Cart: View items, adjust quantities, and checkout.
- Favorites: View and manage favorite items.
- Orders: View, edit, or delete placed orders.
- Admin Panel: Accessible at /admin for adding menu items with images.

- **Project Structure**
<img width="713" height="495" alt="Screenshot 2025-07-23 233816" src="https://github.com/user-attachments/assets/ad53998b-51c4-45fc-9485-09ce034c4237" />

<img width="1919" height="1075" alt="Screenshot 2025-07-23 234311" src="https://github.com/user-attachments/assets/3963005f-dce4-4b0b-a897-d90b94a83bf0" />
<img width="1919" height="1079" alt="Screenshot 2025-07-23 234304" src="https://github.com/user-attachments/assets/a4f22b6a-5f01-4fa6-9b2a-a28d1fa64be9" />

<img width="1919" height="988" alt="Screenshot 2025-07-22 023435" src="https://github.com/user-attachments/assets/841773ea-0bed-4894-8570-fddfa87b9a39" />
<img width="1911" height="989" alt="Screenshot 2025-07-22 023350" src="https://github.com/user-attachments/assets/cc6f5587-259c-4d25-b263-ebb9a1fe2c67" />
<img width="1919" height="1068" alt="Screenshot 2025-07-22 021926" src="https://github.com/user-attachments/assets/ca63ae84-6408-46fd-a5f6-d2301861a238" />
<img width="1919" height="1077" alt="Screenshot 2025-07-22 021917" src="https://github.com/user-attachments/assets/2ee5f04b-94ff-4aec-920a-0a7508c16f07" />
