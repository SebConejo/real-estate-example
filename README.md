# Real Estate Example

A demo real estate listing app with a Vue.js frontend and a Manifest backend.

## Features

- Browse and filter property listings
- Simple backend powered by Manifest
- Example of modern full-stack app structure

---

## Project Structure

```
real-estate-example/
  client/   # Vue.js frontend
  server/   # Manifest backend
```

---

## Getting Started

### Prerequisites

- Node.js (v18+ recommended)
- npm

---

### 1. Backend (Manifest)

1. Install dependencies:

   ```bash
   cd server
   npm install
   ```

2. Start Manifest backend in watch mode:

   ```bash
   npm run manifest
   ```

3. (Optional) Seed the database:
   ```bash
   npm run manifest:seed
   ```

- The backend schema is defined in `server/manifest/backend.yml`.

---

### 2. Frontend (Vue.js)

1. Install dependencies:

   ```bash
   cd ../client
   npm install
   ```

2. Start the development server:
   ```bash
   npm run dev
   ```

- The app will be available at `http://localhost:5173` (default Vite port).

---

## Useful Links

- [Manifest Documentation](https://manifest.build/docs)
- [Vue.js Documentation](https://vuejs.org/)

---

## License

This project is for demo purposes.

---

## Email Sending (Mailgun)

The backend uses [Mailgun](https://www.mailgun.com/) to send inquiry emails (see `server/manifest/handlers/sendInquiryEmail.js`).

### Setup

1. Install Mailgun in the backend:

   ```bash
   cd server
   npm install mailgun-js
   ```

2. Create a `.env` file in the `server` directory with the following variables:
   ```env
   MAILGUN_API_KEY=your-mailgun-api-key
   MAILGUN_DOMAIN=your-mailgun-domain
   ```

Replace the values with your actual Mailgun credentials.
