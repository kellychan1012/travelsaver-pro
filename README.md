# TravelSaver Pro ✈️

TravelSaver Pro is a web application designed to help travelers save at least 15% on travel quotes compared to major online booking sites.

## 🌟 Key Features

- **Interactive Quote Request Form**: Easily capture flight, hotel, traveler, and budget preferences along with existing quote details.
- **Dynamic Savings Calculator**: Instant estimation of potential savings based on selected budget ranges.
- **Google Sheets Integration**: Form submissions automatically submit quote requests to a Google Apps Script webhook / Google Sheet backend.
- **WhatsApp Direct Messaging**: Floating quick-contact widget for fast user inquiry response.
- **Vercel Serverless API**: Backend serverless endpoint (`api/bookings.js`) powered by Prisma ORM for storing booking inquiries.
- **Responsive UI**: Fully mobile-responsive and modern design with clean CSS gradients and interactive feedback.

## 📁 Project Structure

```
.
├── index.html       # Single-page landing site and quote form UI
├── api/
│   └── bookings.js  # Serverless API endpoint (POST) using Prisma ORM
├── vercel.json      # Routing and deployment configuration for Vercel
└── README.md        # Project documentation
```

## 🛠️ Tech Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Backend / Serverless**: Node.js / Vercel Serverless Functions
- **Database / ORM**: Prisma ORM
- **Deployment**: Vercel

## 🚀 Getting Started

### Prerequisites

- A web browser to view the client interface.
- Node.js (v18+) if developing serverless functions locally.

### Local Development

1. **Client**:
   Simply open `index.html` in any web browser, or serve it using a local static file server (e.g., `npx serve .` or VS Code Live Server).

2. **Google Sheets Webhook Setup**:
   - Update `GOOGLE_SCRIPT_URL` in `index.html` with your deployed Google Apps Script URL to receive form submissions directly into a spreadsheet.

3. **API Endpoint Setup**:
   - Ensure Prisma is configured with a database provider (e.g., PostgreSQL or SQLite) in your environment if utilizing the `/api/bookings` serverless route.

## ☁️ Deployment

The project is pre-configured for Vercel deployment via `vercel.json`.

To deploy:
```bash
npx vercel
```

## 📄 License

MIT License.
