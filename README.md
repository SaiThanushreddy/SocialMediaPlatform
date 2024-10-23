# SocialMedia Application

This is a full-stack Twitter-like application. The backend is built using Node.js, Express, GraphQL, Prisma, and AWS S3, while the frontend is built using Next.js, React, Tailwind CSS, and GraphQL code generation.

## Features

### Backend:
- GraphQL API with Apollo Server
- Prisma ORM for database management
- Authentication with JWT
- File storage with AWS S3
- Redis integration for caching or pub/sub

### Frontend:
- React-based user interface using Next.js
- Tailwind CSS for styling
- React Query for data fetching
- Google OAuth for authentication
- GraphQL Code Generator for types and queries

## Technologies

### Backend (Node.js/Express/GraphQL)
- **Express**: Minimal web framework for Node.js
- **GraphQL**: API query language
- **Apollo Server**: GraphQL server
- **Prisma**: ORM for interacting with databases
- **AWS SDK**: Integration with AWS services like S3
- **ioredis**: Redis client for caching and pub/sub
- **JWT (jsonwebtoken)**: Authentication
- **Dotenv**: Environment variable management

### Frontend (Next.js/React)
- **Next.js**: React framework for server-side rendering
- **React Query**: State and server data management
- **Tailwind CSS**: Utility-first CSS framework
- **Google OAuth**: Social login via Google
- **GraphQL Code Generator**: Automatically generates TypeScript types and queries from GraphQL schema

## Getting Started

### Prerequisites
- Node.js
- MongoDB
- AWS Account (for S3)
- Redis (for caching/pub-sub)

### Backend Setup

1. Clone the  repository:

   ```bash
   git clone https://github.com/SaiThanushreddy/SocialMediaPlatform.git
   cd backend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up environment variables by creating a `.env` file in the root directory with the following:

   ```plaintext
   DATABASE_URL=<Your Prisma DB Connection URL>
   JWT_SECRET=<Your JWT Secret>
   AWS_ACCESS_KEY_ID=<Your AWS Access Key>
   AWS_SECRET_ACCESS_KEY=<Your AWS Secret Key>
   AWS_S3_BUCKET=<Your S3 Bucket Name>
   REDIS_URL=<Your Redis Connection URL>
   ```

4. Build and start the backend server:

   ```bash
    npm run dev
   ```

   The backend API will be running on `http://localhost:4000`.

### Frontend Setup

1. Navigate to the frontend repository:

   ```bash
     cd frontend
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Set up environment variables by creating a `.env` file in the root directory with the following:

   ```plaintext
   NEXT_PUBLIC_GRAPHQL_ENDPOINT=http://localhost:4000/graphql
   NEXT_PUBLIC_GOOGLE_CLIENT_ID=<Your Google OAuth Client ID>
   ```

4. Start the development server:

   ```bash
   npm run dev
   ```

   The frontend will be running on `http://localhost:3000`.

## Available Scripts

### Backend Scripts
- `npm start`: Starts the backend server in production mode
- `npm run dev`: Runs the backend server in development mode
- `npm run build`: Compiles the TypeScript code into JavaScript

### Frontend Scripts
- `npm run dev`: Runs the frontend in development mode
- `npm run build`: Builds the frontend for production
- `npm run start`: Starts the frontend in production mode

## Testing the Application

1. Open `http://localhost:3000` in your browser to access the frontend interface.
2. Use Google OAuth to log in, post tweets, and interact with the interface.
3. The GraphQL API can be tested by navigating to `http://localhost:4000/graphql`.
