QuessCorp Employee Management System

Live URL:
https://quesscorplive-ghkd.vercel.app/

A modern Employee Management System built with Next.js App Router and integrated with a Django REST API. The application supports employee listing, searching, attendance tracking, and dashboard analytics with a scalable server/client architecture.

✨ Features

Employee dashboard with key statistics

Search and filter employees using URL query parameters

Employee CRUD operations

Attendance marking and viewing

Server-side rendering with dynamic routing

Optimized build with static and dynamic pages

Production-ready deployment on Vercel

🛠 Tech Stack
Frontend

Next.js 14 (App Router)

React

TypeScript

Tailwind CSS

Lucide Icons

date-fns

Backend

Django

Django REST Framework

Deployment

Vercel (Frontend)

Linux-based server (Django API)

📂 Project Structure (Frontend)
app/
├── page.tsx              # Dashboard (Server Component)
├── attendance/           # Attendance pages
├── employee/             # Employee detail pages
components/
├── employees/            # Employee-related UI components
├── shared/               # Shared UI components
lib/
├── api.ts                # Server-side API calls
├── types.ts              # Type definitions

🔑 Environment Variables

Create a .env.local file in the root directory:

DJANGO_API_URL=https://humhai.in


⚠️ Do not wrap values in quotes
⚠️ Restart the dev server after changing env variables

🚀 Getting Started (Local Development)
1. Install dependencies
npm install

2. Run the development server
npm run dev


App will be available at:

http://localhost:3000

🏗 Build for Production
npm run build
npm start

🌐 Routing Behavior
Route	Type	Description
/	Dynamic	Dashboard with search params
/attendance	Static	Attendance overview
/employee/[id]	Dynamic	Employee profile

Next.js automatically determines static vs dynamic rendering based on data usage.

🧠 Architectural Notes

useSearchParams() is used only in Client Components

Client Components are wrapped in <Suspense> at the Server Component level

All API calls are executed server-side for security and performance

Environment variables are never accessed directly in client code

📦 Deployment

The application is deployed on Vercel using the App Router.

Deployment steps:

Push code to GitHub

Import repository into Vercel

Add environment variables in Vercel dashboard

Deploy

Live URL:
👉 https://quesscorplive-ghkd.vercel.app/

🔒 Security Considerations

Backend API URL is kept server-side

No sensitive keys exposed to the browser

Server Components handle all secure data fetching

📌 Future Enhancements

Pagination and server-side filtering

Role-based access control

Export reports (CSV / PDF)

Attendance analytics charts

Authentication and authorization

👤 Author

Abdul Afjal
Full Stack Developer














This is a [Next.js](https://nextjs.org) project bootstrapped with [`create-next-app`](https://nextjs.org/docs/app/api-reference/cli/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/app/building-your-application/optimizing/fonts) to automatically optimize and load [Geist](https://vercel.com/font), a new font family for Vercel.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/app/building-your-application/deploying) for more details.
