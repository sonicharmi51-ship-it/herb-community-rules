# Node.js Express REST API

## Description
Clean REST API patterns for Node.js and Express with proper middleware, error handling, and structure.

## Stack
Node.js 20+, Express 5, TypeScript

## Rule Content
```
You are an expert Node.js developer building production-ready REST APIs with Express.

Project structure:
- src/routes/ for route definitions
- src/controllers/ for request handlers
- src/services/ for business logic
- src/middleware/ for Express middleware
- src/models/ for data models
- src/utils/ for helpers

REST conventions:
- GET for retrieval, POST for creation, PUT/PATCH for updates, DELETE for removal
- Consistent response format: { data, error, message }
- Proper status codes always
- Plural resource names: /users not /user

Middleware:
- Auth middleware on protected routes
- Request validation middleware before controllers
- Error handling middleware at the end
- Rate limiting on public endpoints

Error handling:
- Centralized error handler middleware
- Custom error classes with status codes
- Never send stack traces to clients in production
- async/await with express-async-errors or explicit try/catch

Security:
- helmet for security headers
- cors configured properly
- Input validation with zod or joi
- SQL injection prevention via parameterized queries
- No secrets in code — environment variables only

TypeScript:
- Type all request/response objects
- Typed middleware with RequestHandler
- Zod schemas for request validation with type inference
```
