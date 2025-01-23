# Backend setup for Noore Todo app

Follow the steps below to set up and run the project locally.

## Prerequisites

Make sure you have the following installed on your system:

- **Node.js** (>= 20.x)
- **npm** (Node Package Manager)

## Getting Started

### Step 1: Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/shashidhar-katkam/noore-todo-backend.git
cd noore-todo-backend
npm install
```

### Step 2: Setup Database

Please update the database connection URL in the .env file. A sample database URL is already provided for demonstration purposes, so there's no need to change it. It will automatically work with AWS RDS.

Run the command below to create the database and tables in the DB instance. If you're not changing the DB URL, you can skip this step.

```bash
npx prisma migrate dev --name init
```

Run the command below for Prisma to generate models.

```bash
npx prisma generate
```

### Step 3: Run the application

Run the below command to run the application.

```bash
npm run dev
```

That's it. You application is running at http://localhost:8998

Thank you.








# Backend setup for Noore Todo app

The Noore Todo Application is a simple todo-list management app that allows users to add, edit, delete, and manage their tasks. It features a frontend developed with React and a backend powered by Node.js. This guide will walk you through the setup and configuration process to get the app up and running.

Follow the steps below to set up and run the project locally.

## Prerequisites

Make sure you have the following installed on your system:

- **Node.js** (>= 20.x)
- **npm** (Node Package Manager)
- Access to the backend repository: [Noore Todo Backend](https://github.com/shashidhar-katkam/noore-todo-backend)
- Setup and run the backend

## Getting Started

### Step 1: Clone the Repository

Clone the repository to your local machine:

```bash
git clone https://github.com/shashidhar-katkam/noore-todo-frontend.git
cd noore-todo-frontend
npm install
```

### Backend URL Configuration

To configure the backend URL for your application, follow these steps:

1. Open the file located at:  
   `app\utils\constants.ts`

2. Locate the section where the backend URL is defined. It should look something like this:

   ```ts
   export const url = "http://127.0.0.1:4000";
   ```

### Step 3: Run the application

Run the below command to run the application.

```bash
npm run dev
```

That's it. You application is running at http://localhost:3000

Thank you.

