
# Sweet Pants Furniture Renting Application

Sweet Pants is a Django-based platform designed for renting furniture, facilitating transactions between renters and customers. It provides essential features for managing inventory, bookings, and user interactions.

https://detrace.systems/ecommerce/

## Features

### Authentication and User Management:
- Separate authentication for renters and customers.
- Renters can manage furniture listings and track booking details.
- Customers can view rental history, manage profiles, and use a wishlist.

### Core Functionality:
- Efficient database models for users, furniture items, bookings, and reviews.
- Renters can add and manage furniture listings, and view booking details.
- Customers can view available items, select rental dates, and place orders.

### Additional Features:
- Integration of Google OAuth for secure sign-in using Django Allauth.
- Email notifications to renters on customer bookings via Mailjet API.
- Migration from SQLite to PostgreSQL for robust data management.
- Renters can generate CSV/Excel reports for rental history analysis.
- Enhanced booking system with shopping cart and wishlist functionalities.

### Deployment:
- Deployed on DigitalOcean using Docker, Nginx, and Gunicorn.
- Configured for scalability and security in production environments.

## Setup

To set up the project:

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/sweetpants.git
   cd sweetpants
   ```

2. Create a `keyconfig.py` file in the same directory as `settings.py`:
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

3. Customize Django settings for your environment (development or production).

4. Set up Django admin groups 'Customer' and 'Renter' for user permissions.

## Usage

Access the application by navigating to the IP address of your DigitalOcean droplet.

For more details and code, visit the [project repository](www.detrace.systems/ecommerce/).

---

This version of the README provides a concise overview of your furniture renting application, focusing on its features, setup instructions, and deployment details.
