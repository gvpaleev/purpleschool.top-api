# PurpleSchool Top API

REST API for an educational platform built with NestJS, MongoDB, and TypeScript.

## Features

- **Authentication & Authorization** - JWT-based authentication with Passport
- **Product Management** - CRUD operations for educational products
- **Reviews System** - User reviews and ratings
- **Top Pages** - Management of landing pages and categories
- **MongoDB Integration** - Using Typegoose for type-safe MongoDB operations

## Tech Stack

- **Framework**: NestJS 10
- **Database**: MongoDB with Mongoose
- **Authentication**: JWT + Passport
- **Validation**: class-validator, class-transformer
- **ODM**: Typegoose
- **Testing**: Jest

## Prerequisites

- Node.js (v18+)
- MongoDB
- npm or yarn

## Installation

```bash
npm install
```

## Configuration

Create a `.env` file in the root directory:

```env
MONGO_URI=mongodb://localhost:27017/purpleschool
JWT_SECRET=your_jwt_secret_key
```

## Running the Application

```bash
# Development mode
npm run start:dev

# Production mode
npm run build
npm run start:prod

# Debug mode
npm run start:debug
```

The API will be available at `http://localhost:3000/api`

## API Modules

### Auth
- User registration and login
- JWT token generation
- Protected routes with guards

### Product
- Create, read, update, delete products
- Product search and filtering

### Review
- Add reviews to products
- Get reviews by product
- Delete reviews

### Top Page
- Manage landing pages
- Category organization

## Testing

```bash
# Unit tests
npm run test

# E2E tests
npm run test:e2e

# Test coverage
npm run test:cov
```

## Code Quality

```bash
# Linting
npm run lint

# Format code
npm run format
```

## Project Structure

```
src/
├── auth/           # Authentication module
├── product/        # Product management
├── review/         # Reviews system
├── top-page/       # Landing pages
├── configs/        # Configuration files
├── decorators/     # Custom decorators
├── pipe/           # Validation pipes
└── main.ts         # Application entry point
```

## License

UNLICENSED
