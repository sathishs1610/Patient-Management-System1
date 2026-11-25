# Patient Management System (Assignment Starter)

## Stack
React + Redux Toolkit + React Router, NestJS, PostgreSQL, Razorpay.

## Prerequisites
Install Node.js (LTS) and PostgreSQL. Create database `patient_management`.

## Run backend
1. Open terminal in `backend`.
2. `npm install`
3. Copy `.env.example` to `.env` and set PostgreSQL credentials.
4. `npm run start:dev`
Backend: http://localhost:3000

## Run frontend
1. Open another terminal in `frontend`.
2. `npm install`
3. Copy `.env.example` to `.env`
4. `npm run dev`
Frontend: Vite will show its local URL, usually http://localhost:5173

## Demo login
admin@hospital.com / Admin@123
The demo login is a frontend fallback for assignment demonstration. Replace with a proper database-backed login and hashed passwords before production.

## Razorpay
Set test credentials in backend `.env`. Never expose `RAZORPAY_KEY_SECRET` in frontend.
Add Razorpay checkout script in frontend/index.html before closing body:
`<script src="https://checkout.razorpay.com/v1/checkout.js"></script>`
Then run the payment flow with Razorpay test mode.

## Notes
This is a runnable assignment starter scaffold, not a production-ready hospital system. Add JWT authentication/guards, robust DTO validation, transaction-safe payment records, Razorpay webhook handling, and full bill edit/delete/payment history to complete every PDF requirement.
