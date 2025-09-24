# Dashboard Template – “Firma”
<img width="1900" height="940" alt="image" src="https://github.com/user-attachments/assets/b2d4a377-7ce4-43de-b842-bb32b5e9b128" />


## 📖 Overview

This repository contains the source files for **Firma**, a responsive admin and dashboard template.  
The template is designed to help developers quickly scaffold out a modern back-office interface for web applications.  
It relies on plain **HTML/CSS/JavaScript** – there is **no build system required** – so you can drop the files onto any web server and begin using the dashboard immediately.  

The default style uses **Bootstrap 4** with a custom colour palette, but alternative themes (**classic, dark, light**) can be selected via a URL parameter or cookie.

---

## ✨ Key Characteristics

- 📱 **Responsive layout** – sidebar collapses on smaller screens; cards and tables reflow gracefully.  
- 🎨 **Clean design** – built on “Nunito Sans” and carefully chosen light/dark palettes.  
- 🗂 **Standalone** – all dependencies bundled in `fonts/`, `js/`, and `css/`.  
- 📑 **Multi-page structure** – includes dashboard, forms, tables, charts, authentication, error pages, and more.

---

## ⚡ Features

- **UI Components**: Alerts, Buttons, Cards, Grid, Modals, Notifications, Tabs, Typography  
- **Charts**: [Chart.js](https://www.chartjs.org/) and [ApexCharts](https://apexcharts.com/)  
- **Forms**:  
  - Basic controls  
  - Advanced widgets (Select2, Date Pickers, Colour Pickers, etc.)  
  - Input Groups, Editors, Validation, Wizard (multi-step forms)  
- **Tables**: Bootstrap Tables, DataTables with search/sort/pagination  
- **Icons**: Feather, Ion Icons, Font Awesome  
- **Utilities**: Calendar, Google Maps, Vector Maps, Pricing Tables, Invoice Pages, Task Management  

### 📂 Example Pages
- **Pages**: Settings, Clients, Invoice, Pricing, Tasks, Blank Page  
- **Authentication**: Sign In, Sign Up, Reset Password, 404/500 error pages  

---

## 🚀 Getting Started

Because the dashboard is a static site, you can run it directly from your filesystem or from any HTTP server.  
Some libraries require an HTTP context, so it’s recommended to use a dev server:

```bash
# From project root
python3 -m http.server 8080

# or with Node.js
npx http-server -p 8080
