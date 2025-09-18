# 📊 Student Analytics Dashboard

The **Student Analytics Dashboard** is a web application built with **Next.js** to visualize student performance metrics and insights. It integrates analysis results generated from **Jupyter Notebooks** and presents them through interactive charts and tables. The project is fully deployable on **Vercel** for easy access.

---

## 🔎 Overview

This project has two main components:

- **Analysis (`analysis/`)**  
  Jupyter Notebooks that process student data, perform statistical analysis, and generate insights. The processed results are exported as JSON files.

- **Dashboard (`dashboard/`)**  
  A **Next.js** application that visualizes the processed JSON data using charts, tables, and key insights.

---

## ✨ Features

- Displays **average metrics**: assessment scores, comprehension, attention, focus, and retention.
- Multiple visualization types:
  - 📊 Bar charts
  - 🔵 Scatter plots
  - 🕸 Radar charts
  - 📑 Interactive student data table
- Provides **key insights** derived from data analysis.
- Static build, optimized for deployment via **Vercel**.

---

## 🚀 Deployment

- **Vercel (Live)**: [https://student-analysis-plum.vercel.app/](https://student-analysis-plum.vercel.app/)  
- **GitHub Repo**: [https://github.com/gowda084/student-analysis](https://github.com/gowda084/student-analysis)

---

## 🛠 Prerequisites

Ensure you have the following installed:

- **Node.js**: `v14.x` or higher  
- **npm**: Comes bundled with Node.js  
- **Git**: For version control & deployment  

---

## ⚙️ Installation & Setup

### 1. Clone the Repository
```bash
git clone https://github.com/gowda084/student-analysis.git
cd student-analytics-dashboard
```

### 2. Navigate to the Dashboard
```bash
cd dashboard
```

### 3. Install Dependencies
```bash
npm install
```

### 4. Run Locally
```bash
npm run dev
```

Now open 👉 [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📂 Project Structure

```
student-analytics-dashboard/
│
├── analysis/                # Jupyter Notebooks for data analysis
│   ├── *.ipynb              # Data processing & insights generation
│   └── output JSON files    # students.json, insights.json
│
├── dashboard/               # Next.js frontend
│   ├── app/                 # Pages & React components
│   │   ├── page.tsx         # Main dashboard page
│   │   └── lib/data.ts      # Data loading logic
│   ├── components/          # Reusable chart & table components
│   └── public/data/         # Static JSON files (students.json, insights.json)
│
├── .gitignore               # Ignore node_modules, .next, etc.
├── vercel.json              # Deployment config for Vercel
```

---

## 📊 Data Files

- **`public/data/students.json`** → Contains student performance metrics (e.g., comprehension, attention, assessment scores).  
- **`public/data/insights.json`** → Contains key insights derived from analysis.

---

## 🚢 Deployment Instructions

1. Ensure `public/data` contains both `students.json` and `insights.json`.  
2. Commit & push changes to GitHub:
   ```bash
   git add .
   git commit -m "Update data & dashboard"
   git push origin main
   ```
3. Deploy to **Vercel**:
   ```bash
   cd dashboard
   vercel --prod
   ```

Your dashboard will be live on your assigned Vercel URL 🎉
