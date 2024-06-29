

# Sweet Pants E-commerce Application

Sweet Pants is an advanced e-commerce platform built with Django, designed to facilitate seamless transactions between vendors and customers. It offers a robust set of features aimed at enhancing functionality and user experience throughout various stages of development.

## Overview

This repository hosts an e-commerce application with comprehensive capabilities:

### Authentication and User Management:

- Utilizes Django's authentication system to manage vendors and customers separately.
- Vendors can register, manage their product listings, and monitor orders associated with their products.
- Customers can register, view order history, and manage their profiles.

### Core Functionality:

- Efficient database models structured for managing users, products, orders, and reviews.
- Supports essential vendor actions such as product management and order tracking.
- Customers can add funds to their accounts and place orders based on available balances and product availability.
- Features a dynamic home page listing all available items, prioritizing top-selling products.

### Additional Features:

- Integration of OAuth for Google sign-in using Django Allauth for enhanced user authentication.
- Automated email notifications to vendors upon customer purchases, powered by the Mailjet API.
- Migration from SQLite to PostgreSQL for robust and scalable database management.
- Vendor-specific reporting capabilities with CSV/Excel exports for detailed sales analysis.
- Advanced ordering system allowing customers to purchase multiple items simultaneously using a shopping cart model.
- Wishlist functionality enabling customers to save desired items for future purchase.

### Deployment:

- Deployed on DigitalOcean using Docker, Nginx, and Gunicorn to ensure a scalable and secure hosting environment.
- Configured for production readiness with customizable Django settings to suit development and production environments.

## Setup

To set up the project locally, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sweetpants.git
   cd sweetpants
   ```

2. Create a `keyconfig.py` file in the same directory as `settings.py` with the following content:
   ```python
   # Django settings
   SECRET_KEY = 'your_secret_key_here'
   DEBUG = True  # Set to False in production

   # Google Allauth
   CLIENT_ID = 'your_google_client_id'
   CLIENT_SECRET = 'your_google_client_secret'

   # Mailjet
   MJ_APIKEY_PUBLIC = 'your_mailjet_public_key'
   MJ_APIKEY_PRIVATE = 'your_mailjet_private_key'
   ```

3. Customize Django settings as per your environment (development or production).

4. Set up Django admin groups 'Customer' and 'Vendor' for user permissions.

## Usage

Access the live application by navigating to the IP address of your DigitalOcean droplet.

## Full-Stack Application for Furniture Renting

For a comprehensive furniture renting application, development involves creating both frontend and backend components to manage user interactions, inventory, payments, and booking processes.

### Core Features

#### User Authentication and Profiles

- Enable user registration, login, and account management.
- Allow users to create profiles, update information, and view rental history.

#### Furniture Listings

- Display a catalog of available furniture items for rent.
- Include detailed item descriptions, rental prices, availability status, and high-quality images.

#### Search and Filter

- Implement search functionality for users to find specific furniture items by keywords, categories, or attributes.
- Provide filtering options based on price range, item type, location, etc.

#### Booking and Reservation

- Enable users to select rental dates, add items to their cart or wishlist, and confirm reservations.
- Manage availability calendars and booking statuses for effective rental management.

#### Payment Integration

- Integrate secure online payment gateways (e.g., UPI, Stripe) to facilitate payment processing for rentals.
- Provide users with payment confirmation and detailed receipts for transparency.

For detailed code and further instructions, visit our [project repository](www.detrace.systems/ecommerce/).

---

This format aims to present a clear and structured overview of your e-commerce application while highlighting its key features and setup instructions for potential users and contributors.
