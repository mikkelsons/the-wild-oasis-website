# The Wild Oasis Website

This is customer-side companion application to [**The Wild Oasis**](https://github.com/mikkelsons/the-wild-oasis) a modern, responsive web application for managing a hotel business. Users can view create an account with Google OAuth and then create reservations, view and edit current reservations, and delete reservations.

### To do:

There is currently no functionality in the app for payments. (This is a fictional business anyways, so who is going to receive the payments? I guess I could take your payments.)

It would be nice for the app to send a confirmation email with booking details, as well as instructions on what the guests need to bring with them. The same goes for deleting a booking, a confirmation email for the deleted booking might be nice.

There is currently no option in the reservation page to add breakfast. The hotel staff can add that later with the internal app (The Wild Oasis, see above), but it might be useful to do that here.

There are undoubtedly many more possible enhancements, but this is just a show project.

## Demo

Try the live app: [The Wild Oasis Website](https://mikkelsons-the-wild-oasis-website.vercel.app/)
You will need to login with Google in order to make reservations and interact with the Guest Area.

## Tech Stack

- **React**: Frontend library for building the user interface.
- **Next.js**: A React framework for server-side rendering. This app uses the App Router for file-based routing and layout management.
- **Supabase**: Database for storing user data, bookings, cabins, and settings.

## Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/mikkelsons/the-wild-oasis.git
   cd the-wild-oasis
   ```

2. Install dependencies:

   ```bash
    npm install
   ```

   or

   ```bash
   yarn install
   ```

3. Start the development server:
   ```bash
   npm run dev
   ```
   or
   ```bash
   yarn dev
   ```
   The app should now be running at http://localhost:3000

## Environment Variables

Create a `.env.local` file in the root directory and add the following:

```bash
SUPABASE_URL=your-supabase-url
SUPABASE_HOST=your-supabase-host
SUPABASE_KEY=your-supabase-anon-key
NEXTAUTH_URL=http://localhost:3000
NEXTAUTH_SECRET=your-next-auth-secret
AUTH_GOOGLE_ID=your-google-auth-id
AUTH_GOOGLE_SECRET=your-google-auth-secret
```

## Acknowledgements

Built as part of [The Ultimate React Course 2025](https://www.udemy.com/course/the-ultimate-react-course/) by Jonas Schmedtmann.
