# The Hunger Cafe

A mobile-first full-stack cafe ordering application with:

- React + Tailwind CSS frontend
- Node.js + Express backend
- MongoDB + Mongoose database
- Razorpay test-mode payment support
- Role-based admin dashboard
- Customer phone login with demo OTP verification

## Project Structure

```text
client/   React application
server/   Express API
```

## Run Locally

1. Install frontend packages:

   ```bash
   npm run install:client
   ```

2. Install backend packages:

   ```bash
   npm run install:server
   ```

3. Create environment files:

   - `server/.env`
   - `client/.env`

4. Start the backend:

   ```bash
   npm run dev:server
   ```

5. Start the frontend:

   ```bash
   npm run dev:client
   ```

## Backend Environment Variables

```env
PORT=5000
MONGO_URI=mongodb+srv://your-connection-string
JWT_SECRET=replace-with-a-long-secret
RAZORPAY_KEY_ID=rzp_test_xxxxxxxx
RAZORPAY_KEY_SECRET=xxxxxxxx
CLIENT_URL=http://localhost:5173
ADMIN_USERNAME=admin
ADMIN_PASSWORD=changeme123
ADMIN_EMAIL=xyz@gmail.com
OTP_EXPIRY_MINUTES=10
```

## Frontend Environment Variables

```env
VITE_API_BASE_URL=http://localhost:5000/api
VITE_WHATSAPP_NUMBER=918251038187
VITE_UPI_ID=yourupi@upi
```

## Key Features

- Single-site architecture with React Router
- Landing page, ordering flow, and admin dashboard
- Cart persistence using `localStorage`
- Admin JWT authentication
- Customer JWT session after OTP verification
- Razorpay checkout with signature verification
- UPI deep link support
- WhatsApp ordering shortcut
- Demo OTP display for customer login and admin password resets

## Deployment Targets

- Frontend: Vercel
- Backend: Render or Railway
- Database: MongoDB Atlas
