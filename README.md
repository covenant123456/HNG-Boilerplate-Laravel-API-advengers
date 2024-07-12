# HNG Boilerplate Laravel Project

## Table of Contents
- [Introduction](#introduction)
- [Project Structure](#project-structure)
- [API Design](#api-design)
- [Database Design](#database-design)
- [Team Members](#team-members)
- [Getting Started](#getting-started)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Welcome to the HNG Boilerplate Laravel Project! This project aims to create a robust and secure boilerplate for Laravel applications, incorporating various essential features such as authentication, payments, messaging, user and organization management, and more.

## Project Structure
The project follows a proper structure according to the norms of the Laravel framework. Below are the main features included:

- **Authentication**: Supports traditional login, social authentication, and magic link authentication.
- **Messaging**: Email messaging with default templates and background processing.
- **Payments**: Integrations with Stripe, Flutterwave, and LemonSqueezy.
- **User & Organization Management**: Features for managing users and organizations, including superadmin interfaces.
- **Settings**: Profile settings, application settings, and more.
- **Dashboards**: Basic user and admin dashboards.
- **Notifications**: Real-time notifications.
- **Content Management**: Blog, content editing, and more.
- **GDPR Compliance**: GDPR cookie consent management.
- **Data Export**: User data export functionality.

## API Design
The API design is crafted using OpenAPI standards. It includes endpoints for authentication, user and organization management, payments, messaging, notifications, and more. Below is an overview of the API endpoints:

- **Authentication**:
  - `POST /api/auth/login`: User login
  - `POST /api/auth/register`: User registration
  - `POST /api/auth/social`: Social authentication
  - `POST /api/auth/magic-link`: Magic link authentication

- **Users**:
  - `GET /api/users`: List all users
  - `GET /api/users/{id}`: Get a single user
  - `PUT /api/users/{id}`: Update user details
  - `DELETE /api/users/{id}`: Delete a user

- **Organizations**:
  - `GET /api/organizations`: List all organizations
  - `GET /api/organizations/{id}`: Get a single organization
  - `POST /api/organizations`: Create a new organization
  - `PUT /api/organizations/{id}`: Update organization details
  - `DELETE /api/organizations/{id}`: Delete an organization

- **Payments**:
  - `POST /api/payments`: Create a new payment
  - `GET /api/payments`: List all payments

- **Messaging**:
  - `POST /api/messages`: Send a message
  - `GET /api/messages`: List all messages

- **Notifications**:
  - `GET /api/notifications`: List all notifications

- **Content Management**:
  - `GET /api/blog-posts`: List all blog posts
  - `POST /api/blog-posts`: Create a new blog post

For detailed API documentation, please refer to the [Swagger Documentation](https://covenant123456.github.io/HNG-Boilerplate-Laravel-API-advengers/).

## Database Design
The database is designed to support the various features of the application. Below is an overview of the database schema:

### Tables
- **users**: Stores user information.
- **organizations**: Stores organization information.
- **auth_logs**: Logs authentication activities.
- **magic_links**: Stores magic link tokens.
- **messages**: Stores messages.
- **email_templates**: Stores email templates.
- **payments**: Stores payment transactions.
- **user_settings**: Stores user-specific settings.
- **org_settings**: Stores organization-specific settings.
- **notifications**: Stores notifications.
- **blog_posts**: Stores blog posts.
- **invitations**: Stores invitation details.
- **waitlist**: Stores waitlist information.
- **gdpr_cookies**: Stores GDPR cookie consents.
- **data_exports**: Stores data exports.
- **random_data**: Stores random data associated with users.
- **other_data**: Stores miscellaneous data.
- **charts**: Stores chart data.
- **content_edit**: Stores content editing logs.

### Relationships
- Users have many blog posts, messages, notifications, etc.
- Organizations have many users and settings.
- Payments can be associated with both users and organizations.
- Invitations and waitlists reference email templates.

For a detailed database schema, please refer to the [Database Schema](https://dbdiagram.io/d/Copy-of-HNG-Task-3-6691b5829939893daececa72).

## Team Members
- [Member 1 Covenant12 3️⃣](covenantekundayo@gmail.com)
- [Member 2 Redington 3️⃣](nobleehart8@gmail.com)
- [Member 3 Aarondio](dikaaron33@gmail.com)
- [Member 4 amowogbaje3️⃣ ](amowogbajegideon@gmail.com)
- [Member 5 Power3️⃣ ](powerbabaniyi32@gmail.com)

## Getting Started
To get started with the project, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/covenant123456/HNG-Boilerplate-Laravel-API-advengers/
   cd HNG-Boilerplate-Laravel-API-advengers
