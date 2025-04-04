

# **Homestay Hub**  

Homestay Hub is a web-based platform designed to simplify the process of booking and managing homestays. It allows users to browse, book, and manage accommodations while providing hosts with an efficient way to list and manage their properties.  

## **Tech Stack**  

- **Frontend:** React.js, JavaScript  
- **Backend:** Node.js, Express.js  
- **Database:** MongoDB (Cluster with three collections: `users`, `bookings`, `properties`)  
- **Authentication:** JWT (JSON Web Token)  
- **Email Service:** Nodemailer  

## **Features**  

### **User Features**  
✅ User Registration & Login (JWT Authentication)  
✅ Browse and Search for Homestays  
✅ Book Accommodations & Manage Trips  
✅ Receive Email Notifications for:  
   - Account creation  
   - Successful login  
   - Booking confirmation  
   - Cancellation confirmation  

### **Host Features**  
✅ List Properties for Booking  
✅ Manage Listed Properties (Edit, Update, Remove)  
✅ View and Manage Bookings  

### **Admin Features**  
✅ Manage Users, Hosts, and Properties  
✅ Oversee Platform Operations  

## **Database Structure (MongoDB)**  

The database is structured as a **MongoDB cluster** with three main collections:  

1. **Users Collection (`users`)**  
   - Stores user details (name, email, password, role)  
   - JWT-based authentication for security  

2. **Bookings Collection (`bookings`)**  
   - Stores booking details (user ID, property ID, check-in/out dates, status)  
   - Allows users to manage and cancel bookings  

3. **Properties Collection (`properties`)**  
   - Stores details about homestays (location, price, amenities, host details)  
   - Enables hosts to add, edit, and delete property listings  

## **Installation & Setup**  

1. **Clone the Repository**  
   ```sh
   git clone https://github.com/lalit-rg/Homestay-Hub.git  
   cd Homestay-Hub  
   ```  

2. **Backend Setup**  
   ```sh
   cd backend  
   npm install  
   npm start  
   ```  
   - Set up your MongoDB URI and JWT secret in `.env`  

3. **Frontend Setup**  
   ```sh
   cd frontend  
   npm install  
   npm start  
   ```  

## **Future Enhancements**  

- AI-based recommendations for personalized homestay suggestions  
- Multilingual support  
- Enhanced security features  
