
# PayUp Web App

The **PayUp Web App** is a platform designed to manage invoices and facilitate early payments for vendors. It provides an intuitive user interface for creating, tracking, and managing invoices, ensuring a seamless experience for both vendors and users.

## Features
- **Invoice Management**: Create, track, and manage invoices easily.
- **Payment Integration**: Facilitate early payments to vendors.
- **User Authentication**: Secure login and user management.
- **Database**: Built on **PostgreSQL** for reliable data storage.
- **Dockerized Deployment**: Simplifies deployment across different environments.

## Technologies Used
- **Frontend**: 
  - **Next.js**
  - **TypeScript**
- **Backend**:
  - **Express.js**
  - **PostgreSQL**
  - **Prisma** for ORM
- **Deployment**:
  - **Docker**

## Getting Started

### Prerequisites
- **Node.js** (v14 or above)
- **Docker** (for containerization)

### Setup

1. Clone this repository:
   ```bash
   git clone https://github.com/rsharma828/payUp-webapp.git
   cd payUp-webapp
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the root directory and add the required environment variables:
   ```
   DATABASE_URL=your_database_url
   JWT_SECRET=your_jwt_secret
   ```

4. Run migrations (PostgreSQL):
   ```bash
   npx prisma migrate dev
   ```

5. Start the development server:
   ```bash
   npm run dev
   ```

The app will be running on `http://localhost:3000`.

### Docker Setup

1. Build the Docker image:
   ```bash
   docker build -t payup-webapp .
   ```

2. Run the Docker container:
   ```bash
   docker run -p 3000:3000 payup-webapp
   ```

The app will be accessible at `http://localhost:3000`.

## Contributing

If you'd like to contribute, feel free to fork the repository and create a pull request. Please make sure to follow the coding conventions and write tests for new features.

```
