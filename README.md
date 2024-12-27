# My Node.js App

This project is a Node.js application that uses Express for the web framework and MySQL for the database.

## Project Structure

```env
my-nodejs-app
├── server.js 
├── Dockerfile           # Dockerfile for building the application image
├── package.json         # npm configuration file
├── .env                 # Environment variables for the application
└── README.md            # Project documentation
```

## Setup Instructions

1. **Clone the repository**:

   ```bash
   git clone <repository-url>
   cd my-nodejs-app
   ```

2. **Install dependencies**:

   Make sure you have Node.js and npm installed. Run the following command to install the required packages:

   ```bash
   npm install
   ```

3. **Configure environment variables**:

   Create a `.env` file in the root directory and add your database connection details:

   ```env
   DB_HOST=your_database_host
   DB_USER=your_database_user
   DB_PASSWORD=your_database_password
   DB_NAME=your_database_name
   ```

4. **Run the application**:
   You can start the server by running:

   ```bash
   npm start
   ```

## Docker Instructions

To build and run the application using Docker, follow these steps:

1. **Build the Docker image**:

   ```bash
   docker build -t my-nodejs-app .
   ```

2. **Run the Docker container**:

   ```bash
   docker run -p 3000:3000 --env-file .env my-nodejs-app
   ```

## Usage

Once the server is running, you can access the application at `http://localhost:3000` .
