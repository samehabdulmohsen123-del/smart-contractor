# Smart Moqawel

A MERN-style construction cost estimator app with:

- React + Vite frontend
- Tailwind CSS styling
- RTL Arabic support
- Express backend API for estimation logic

## Run Locally

1. Install dependencies
   - `npm install`
   - `cd client && npm install`
   - `cd server && npm install`
2. (Optional) Configure MongoDB
   - Copy `.env.example` to `.env`
   - Set `MONGO_URI` to your MongoDB connection string
3. Start both apps
   - `npm run dev`
4. Open frontend
   - `http://localhost:5173`

## Backend API

- POST `/api/estimate`
  - body: `{ country, livingRoomArea, bedroomArea, bathroomArea, kitchenArea, level }`

## Notes

- The estimator uses sample material formulas and cost factors adjusted by country multipliers.
- The backend includes optional MongoDB persistence for estimate history.
- Country multipliers: Egypt (1x), Saudi Arabia (1.3x), UAE (1.5x)
