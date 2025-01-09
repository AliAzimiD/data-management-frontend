# Data Management Frontend

This repository contains the frontend application for the Enhanced Data Management Application. The frontend allows users to define custom data types and fields, manage rows, apply filters, and import/export data in CSV format.

## Tech Stack

- **React**: JavaScript library for building user interfaces
- **TypeScript**: Typed superset of JavaScript
- **Redux Toolkit**: State management library
- **Axios**: HTTP client for API integration
- **React Hook Form**: Form management
- **Yup**: Schema validation for forms
- **TailwindCSS**: Utility-first CSS framework for styling
- **Jest**: Unit testing framework
- **Cypress**: End-to-end testing framework

## Features

- Dynamic form handling for user-defined types and fields
- Advanced filtering options, including range filters
- CSV import/export functionality
- History tracking of selected rows
- Responsive UI with TailwindCSS

## Setup Instructions

1. **Clone the repository**:
   ```bash
   git clone https://github.com/your-org/data-management-frontend.git
   cd data-management-frontend


2.  **Install dependencies**:
    
    ```bash
    npm install
    ```
    
3.  **Configure environment variables**: Create a `.env` file based on `.env.example`:
    
    ```plaintext
    REACT_APP_API_URL=http://localhost:3000/api
    ```
    
4.  **Run the application**:
    
    ```bash
    npm start
    ```
    
5.  **Run tests**:
    
    ```bash
    npm test
    ```
    

Folder Structure
----------------

```plaintext
src/
├── components/        # UI components
├── hooks/             # Custom React hooks
├── pages/             # Main page components
├── services/          # API service layer
├── store/             # Redux store and slices
├── styles/            # Global and component styles
├── utils/             # Utility functions
└── App.tsx            # Main app component
```
