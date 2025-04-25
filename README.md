# Horizon Banking Platform

Welcome to the Horizon Banking Platform, a modern financial SaaS application developed by Aman Gaur. This project is designed to help users manage multiple bank accounts, track transactions in real-time, transfer funds, and gain insights into their financial activities. Follow the detailed guide below to set up and explore the project!

📋 **Table of Contents**
- [Introduction](#introduction)
- [Tech Stack](#tech-stack)
- [Features](#features)
- [Quick Start](#quick-start)
- [Code Snippets](#code-snippets)
- [Assets](#assets)
- [Contributing](#contributing)
- [Contact](#contact)

## 🤖 Introduction

Horizon is a financial SaaS platform built from scratch by Aman Gaur. It allows users to connect multiple bank accounts, view real-time transactions, transfer funds to other users, and manage their finances seamlessly. The project emphasizes clean code architecture, scalability, and a user-friendly experience.

For support or to report bugs, feel free to reach out via the contact details below or join the open-source community on GitHub.

## ⚙️ Tech Stack

- **Next.js**: React framework for server-side rendering and static site generation
- **TypeScript**: Strongly-typed JavaScript for better code reliability
- **Appwrite**: Backend-as-a-service for authentication and database management
- **Plaid**: API for secure bank account integration
- **Dwolla**: Payment API for fund transfers
- **React Hook Form**: Form management with validation
- **Zod**: Schema validation for TypeScript
- **TailwindCSS**: Utility-first CSS framework
- **Chart.js**: Interactive data visualization
- **ShadCN**: Reusable UI components

## 🔋 Features

- **Secure Authentication**: Server-side rendered authentication with robust validation and authorization
- **Bank Integration**: Connect multiple bank accounts using Plaid
- **Dashboard**: View total balance, recent transactions, and spending categories
- **Bank Management**: List all connected banks with account details and balances
- **Transaction History**: Paginated and filterable transaction records
- **Real-Time Updates**: Instant reflection of new bank connections across the app
- **Fund Transfers**: Transfer money to other users via Dwolla with secure validation
- **Responsive Design**: Optimized for desktop, tablet, and mobile devices
- **Code Reusability**: Modular architecture for maintainability and scalability

## 🤸 Quick Start

Follow these steps to set up the Horizon Banking Platform locally.

### Prerequisites

Ensure you have the following installed:
- Git
- Node.js
- npm (Node Package Manager)

### Cloning the Repository

```bash
git clone https://github.com/amangaur/horizon-banking.git
cd horizon-banking
```

### Installation

Install dependencies using npm:

```bash
npm install
```

### Set Up Environment Variables

Create a `.env` file in the project root and add the following:

```
# NEXT
NEXT_PUBLIC_SITE_URL=

# APPWRITE
NEXT_PUBLIC_APPWRITE_ENDPOINT=https://cloud.appwrite.io/v1
NEXT_PUBLIC_APPWRITE_PROJECT=
APPWRITE_DATABASE_ID=
APPWRITE_USER_COLLECTION_ID=
APPWRITE_BANK_COLLECTION_ID=
APPWRITE_TRANSACTION_COLLECTION_ID=
APPWRITE_SECRET=

# PLAID
PLAID_CLIENT_ID=
PLAID_SECRET=
PLAID_ENV=
PLAID_PRODUCTS=
PLAID_COUNTRY_CODES=

# DWOLLA
DWOLLA_KEY=
DWOLLA_SECRET=
DWOLLA_BASE_URL=https://api-sandbox.dwolla.com
DWOLLA_ENV=sandbox
```

Replace placeholders with credentials from [Appwrite](https://appwrite.io/), [Plaid](https://plaid.com/), and [Dwolla](https://www.dwolla.com/).

### Running the Project

```bash
npm run dev
```

Open `http://localhost:3000` in your browser to view the application.

## 🕸️ Code Snippets

Key components and utilities include:
- `.env.example`: Template for environment variables
- `exchangePublicToken`: Handles Plaid token exchange
- `user.actions.ts`: User-related backend logic
- `dwolla.actions.ts`: Dwolla payment processing
- `bank.actions.ts`: Bank connection management
- `BankTabItem.tsx`: UI for bank tabs
- `BankInfo.tsx`: Displays bank details
- `Copy.tsx`: Copy-to-clipboard utility
- `PaymentTransferForm.tsx`: Fund transfer form
- `BankDropdown.tsx`: Bank selection dropdown
- `Pagination.tsx`: Transaction history pagination
- `Category.tsx`: Spending category visualization

Refer to the repository for complete code.

## 🔗 Assets

Assets (icons, images, etc.) are available in the `/public/assets` directory. Additional resources can be found [here](https://github.com/amangaur/horizon-banking/assets).

## 🚀 Contributing

Contributions are welcome! Please follow these steps:
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit changes (`git commit -m 'Add your feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a pull request

## 📬 Contact

For inquiries, reach out to Aman Gaur at:
- Email: aman.gaur@example.com
- GitHub: [amangaur](https://github.com/amangaur)

Thank you for exploring the Horizon Banking Platform! 🚀
