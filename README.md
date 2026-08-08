# Spendwise

### Know where your money goes.

Spendwise is a modern, local-first expense tracker designed to make everyday spending easier to record, understand, and manage.

It provides a focused dashboard for tracking expenses, reviewing spending patterns, setting monthly category budgets, and exporting records — without requiring an account or a backend.

**[Live Demo](https://spendwise-beta-five.vercel.app)** · **[GitHub Repository](https://github.com/Mk-Zone14/spendwise)**

---

## ✨ Features

* **Expense management** — Add, edit, and delete expenses with amount, description, category, and date.
* **Spending dashboard** — View total spending, transaction count, and the category receiving the most spending.
* **Category breakdown** — Visualize spending allocation across categories with an interactive chart.
* **Smart filtering** — Search expenses, filter by category, and switch between predefined date ranges.
* **Date ranges** — Quickly view spending for today, this week, this month, the last 30 days, or all time.
* **Monthly budgets** — Set category-level monthly spending limits and monitor progress toward each limit.
* **CSV export** — Export the currently visible expense records as a CSV file.
* **Light & dark mode** — Switch between color modes based on preference.
* **Local-first storage** — Expense data, budgets, and theme preferences are stored locally in the browser.
* **No account required** — No authentication or external database is needed to use the application.

---

## 🛠️ Tech Stack

| Technology               | Purpose                                         |
| ------------------------ | ----------------------------------------------- |
| **React**                | UI and application state                        |
| **Vite**                 | Development server and production build tooling |
| **Tailwind CSS**         | Styling infrastructure                          |
| **Lucide React**         | Interface icons                                 |
| **JavaScript**           | Application logic                               |
| **Browser localStorage** | Local data persistence                          |
| **Vercel**               | Production deployment                           |

---

## 🧠 How It Works

Spendwise is intentionally client-side.

Expense records and monthly budgets are maintained in React state and persisted to the browser using `localStorage`. Derived values such as totals, category breakdowns, filtered records, and budget progress are calculated from the current application state.

There is no application server, external database, or authentication layer.

This keeps the project lightweight and means personal expense data stays in the browser being used.

### Data stored locally

Spendwise currently stores:

* Expense records
* Monthly category budgets
* Color-mode preference

Because the data is browser-local, it is **not synchronized between devices or browsers**.

Clearing the browser's site data can also remove locally stored expense information.

---

## 📊 Expense Categories

Spendwise currently supports:

* Food & Dining
* Transport
* Education
* Entertainment
* Shopping
* Health
* Other

---

## 🚀 Getting Started

### Prerequisites

You need:

* Node.js
* npm

### Installation

Clone the repository:

```bash
git clone https://github.com/Mk-Zone14/spendwise.git
cd spendwise
```

Install dependencies:

```bash
npm install
```

Start the development server:

```bash
npm run dev
```

Vite will provide a local development URL in the terminal.

---

## 🧪 Available Scripts

### Development

```bash
npm run dev
```

Starts the Vite development server.

### Production build

```bash
npm run build
```

Creates the optimized production build.

### Lint

```bash
npm run lint
```

Runs Oxlint against the project.

### Preview

```bash
npm run preview
```

Serves the production build locally for previewing.

---

## 📁 Project Structure

```text
spendwise/
├── public/
│   └── ...
├── src/
│   ├── assets/
│   ├── App.jsx
│   ├── index.css
│   └── main.jsx
├── .gitignore
├── .oxlintrc.json
├── index.html
├── package.json
├── package-lock.json
├── vercel.json
└── vite.config.js
```

The application currently keeps its core UI and state logic in `src/App.jsx`, with styling in `src/index.css`.

---

## 🔒 Privacy & Limitations

Spendwise does not currently send expense data to a remote server.

That makes the application simple and privacy-friendly, but it also comes with trade-offs:

* Data is tied to the current browser/device.
* There is no cloud synchronization.
* There is no user account system.
* There is no cross-device backup.
* Clearing browser storage can remove locally saved data.

This is a deliberate trade-off of the current client-side architecture rather than a substitute for a cloud-backed financial application.

---

## 🌱 Possible Future Improvements

Potential directions for future versions include:

* Cloud synchronization
* Optional user accounts
* Recurring expenses
* Custom categories
* More detailed spending analytics
* Budget notifications
* Importing existing CSV records
* Data backup and restore
* More flexible date-range filtering
* Automated tests and end-to-end testing

These are intentionally outside the scope of the current version.

---

## 🎯 Project Goals

Spendwise was built around a simple idea:

> Expense tracking should make spending easier to understand, not create another source of friction.

The project focuses on a small, responsive interface, useful derived insights, local persistence, and straightforward interaction rather than adding complexity for its own sake.

---

## 📄 License

This project is currently maintained as a personal portfolio project.
