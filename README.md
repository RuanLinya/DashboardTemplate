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
<img width="1905" height="940" alt="image" src="https://github.com/user-attachments/assets/538360c5-529b-4671-8be0-aa6c9bf489be" />
<img width="1903" height="935" alt="image" src="https://github.com/user-attachments/assets/18f68de8-d34b-44ad-a894-0f93c7900b00" />
<img width="1900" height="904" alt="image" src="https://github.com/user-attachments/assets/d33055d2-aedc-4d5a-97a7-3f769411ecd0" />
<img width="1898" height="937" alt="image" src="https://github.com/user-attachments/assets/7c2b0523-6239-40cd-a551-e7381b18d61f" />
<img width="1900" height="936" alt="image" src="https://github.com/user-attachments/assets/b4c85dc6-57bd-454d-8a47-0732bb96b00a" />
<img width="1903" height="731" alt="image" src="https://github.com/user-attachments/assets/03f1cdff-46dd-464f-99e9-b440545747dc" />

- **Authentication**: Sign In, Sign Up, Reset Password, 404/500 error pages
<img width="675" height="610" alt="image" src="https://github.com/user-attachments/assets/2564bbf7-a5d5-495e-a0fe-5d06509d097a" />
<img width="656" height="597" alt="image" src="https://github.com/user-attachments/assets/caa1ff03-3ac2-4e36-bd5e-33991d3e5cfd" />
<img width="701" height="333" alt="image" src="https://github.com/user-attachments/assets/f04bdeb2-cc84-4881-8f5d-dd32becdfaa0" />
<img width="582" height="320" alt="image" src="https://github.com/user-attachments/assets/bc23c0e7-dba7-4ced-acf9-7c626d94eebe" />
<img width="679" height="330" alt="image" src="https://github.com/user-attachments/assets/922031a4-8149-413f-a706-635f902791c3" />






---

## 🚀 Getting Started

Because the dashboard is a static site, you can run it directly from your filesystem or from any HTTP server.  
Some libraries require an HTTP context, so it’s recommended to use a dev server:

```bash
# From project root
python3 -m http.server 8080

# or with Node.js
npx http-server -p 8080
