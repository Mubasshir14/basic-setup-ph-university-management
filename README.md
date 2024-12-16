# PH UNIVERSITY MANAGEMENT

## Description
This project is a Node.js application with TypeScript support, designed to provide a backend service using Express.js and MongoDB.

## Features
- TypeScript for strong typing and enhanced developer experience.
- Express.js for creating the server and APIs.
- MongoDB for database management using Mongoose.
- Environment variable management with `dotenv`.
- Authentication using JSON Web Tokens (JWT) and `bcrypt` for password hashing.
- Linting and formatting with ESLint and Prettier.
- Pre-commit hooks with Husky and lint-staged.
- Modular architecture for scalability.

## Prerequisites
Make sure you have the following installed:
- **Node.js** (version 16 or above)
- **npm** or **yarn**
- **MongoDB instance** (local or cloud-based)

## Installation

1. **Clone the repository:**
   ```bash
   git clone <repository-url>
   cd <repository-folder>
   ```

2. **Install dependencies:**
   ```bash
   npm install
   ```

3. **Create a `.env` file** in the root directory and configure your environment variables:
   ```env
   PORT=3000
   DATABASE_URL= your-mongodb-uri
   BCRYPT_SALT_ROUND= any-number
   DEFAULT_PASS= default-pass
   JWT_ACCESS_SECRET = your-secret-key
   JWT_REFRESH_SECRET = your-secret-key
   JWT_ACCESS_EXPIRES_IN= your-time
   JWT_REFRESH_EXPIRES_IN= your-time
   ```

## Scripts

- **Start Development Server:**
  ```bash
  npm run start:dev
  ```

- **Build for Production:**
  ```bash
  npm run build
  ```

- **Start Production Server:**
  ```bash
  npm run start:prod
  ```

- **Lint Code:**
  ```bash
  npm run lint
  ```

- **Fix Lint Issues:**
  ```bash
  npm run lint:fix
  ```

- **Fix Formatting Issues:**
  ```bash
  npm run format
  ```

## Folder Structure
```
├── src
│   ├── controllers     # Request handlers
│   ├── models          # Mongoose models
│   ├── routes          # Express routes
│   ├── middleware      # Custom middleware
│   ├── utils           # Helper functions
│   └── server.ts       # Entry point of the application
├── dist                # Compiled JavaScript files
├── .eslintrc.json      # ESLint configuration
├── .prettierrc         # Prettier configuration
├── tsconfig.json       # TypeScript configuration
└── package.json        # Project metadata and scripts
```

## Dependencies

### Production:
- `bcrypt`: Password hashing library
- `cookie-parser`: Parse cookies for HTTP requests
- `cors`: Enable Cross-Origin Resource Sharing
- `dotenv`: Load environment variables from `.env` file
- `express`: Web framework for Node.js
- `http-status`: Utility for HTTP status codes
- `jsonwebtoken`: Handle JWT authentication
- `mongoose`: MongoDB object modeling tool
- `zod`: TypeScript-first schema validation

### Development:
- `typescript`: TypeScript compiler
- `eslint`: Linting tool for JavaScript/TypeScript
- `prettier`: Code formatter
- `ts-node-dev`: Development server for TypeScript
- `husky`: Pre-commit hooks

## Contributing
Contributions are welcome! Please follow these steps:

1. **Fork the repository.**
2. **Create a new branch** for your feature or bugfix.
3. **Commit your changes** with descriptive messages.
4. **Push your changes** and open a pull request.

---
