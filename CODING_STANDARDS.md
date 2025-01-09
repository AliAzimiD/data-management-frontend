# Coding Standards for Data Management Application

This document outlines the coding standards for both backend and frontend development in the Data Management Application. Following these standards ensures code consistency, readability, and maintainability across the project.

## General Coding Guidelines

1. **Language**:
   - **Backend**: Node.js with TypeScript
   - **Frontend**: React with TypeScript
2. **Formatting**:
   - Use **Prettier** for automatic code formatting.
   - Prettier configuration:
     ```json
     {
       "semi": true,
       "singleQuote": true,
       "trailingComma": "es5",
       "printWidth": 80,
       "tabWidth": 2
     }
     ```
3. **Linting**:
   - Use **ESLint** with recommended rules for TypeScript and React.
   - ESLint configuration:
     ```json
     {
       "extends": [
         "eslint:recommended",
         "plugin:@typescript-eslint/recommended",
         "plugin:react/recommended",
         "prettier"
       ],
       "parser": "@typescript-eslint/parser",
       "plugins": ["@typescript-eslint", "react"],
       "rules": {
         "no-unused-vars": "warn",
         "react/prop-types": "off"
       }
     }
     ```
4. **Code Comments**:
   - Add comments for complex or non-obvious logic.
   - Use JSDoc-style comments for functions and methods:
     ```typescript
     /**
      * Fetches all types from the database.
      * @returns {Promise<Type[]>} A promise that resolves to an array of types.
      */
     async function getAllTypes(): Promise<Type[]> {
       // Logic here
     }
     ```
5. **Naming Conventions**:
   - Use **camelCase** for variables and functions.
   - Use **PascalCase** for class and component names.
   - Use **UPPER_SNAKE_CASE** for constants.

## Backend Coding Standards

1. Use **async/await** for all asynchronous operations.
2. Handle errors using a centralized error-handling middleware.
3. Separate business logic into services and controllers.
4. Use environment variables for sensitive data (`dotenv`).
5. Write unit tests using **Jest** with at least 80% coverage.

### Example Folder Structure

```plaintext
src/
├── controllers/      # Route controllers
├── services/         # Business logic
├── models/           # Database models (Prisma)
├── middlewares/      # Express middlewares
├── routes/           # API routes
└── index.ts          # Main entry point
```
## Frontend Coding Standards
1. Use React Functional Components and React Hooks.
2. Manage global state using Redux Toolkit.
3. Validate forms using React Hook Form and Yup.
4. Ensure components are reusable and well-documented.
5. Write unit and integration tests using Jest and React Testing Library.

### Example Folder Structure
```plaintext
src/
├── components/        # UI components
├── hooks/             # Custom React hooks
├── pages/             # Main page components
├── services/          # API service layer
├── store/             # Redux store
├── styles/            # Global and component styles
└── App.tsx            # Main app component
Testing
Backend:
Use Jest for unit and integration tests.
Write tests for all services and controllers.
Frontend:
Use Jest and React Testing Library for unit and integration tests.
Write tests for all critical components and services.
go
Copy code

---

