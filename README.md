Dashboard Template
Overview

This repository contains the source files for Firma, a responsive admin and dashboard template.
The template is designed to help developers quickly scaffold out a modern back‑office interface for web applications.
It relies on plain HTML/CSS/JavaScript – there is no build system required – so you can drop the files onto any web server and begin using the dashboard immediately.
The default style uses Bootstrap 4 with a custom colour palette, but alternative themes (classic, dark and light) can be selected via a URL parameter or cookie.

Key characteristics

Responsive layout. The sidebar collapses on smaller screens, and the cards and tables reflow gracefully for mobile and tablet displays.

Clean design. Uses the "Nunito Sans" typeface and a carefully chosen colour palette that works across light and dark themes.

Standalone. All dependencies (fonts, icons, JavaScript libraries) are bundled into the fonts/, js/ and css/ folders. There is no need to run a package manager or build step.

Multi‑page structure. The template ships with a collection of ready‑made pages such as a dashboard, forms demos, tables, charts, user authentication, error pages and more (see the Features section below).

Features

The navigation menu illustrates the breadth of components included in this template.
Under Elements you can find user‑interface components such as alerts, buttons, cards, grids, modals, notifications, tabs and typography.
Two charting libraries, Chart.js and ApexCharts, are provided for drawing dashboards and spark‑lines.
The Forms section contains multiple demos: basic form controls, advanced widgets (date pickers, select2 inputs, colour pickers, etc.), input groups, WYSIWYG editors, validation examples and a multi‑step form wizard.
Table examples include both simple Bootstrap tables and fully interactive DataTables with sorting, searching and pagination.
Three icon sets (Feather, Ion Icons and Font Awesome) are available.
Additional utilities include a calendar component, Google and vector map demos, pricing tables, invoice pages and task management screens.

The Pages section of the navigation provides concrete examples that could be used in a real application: settings page, clients table, invoice view, pricing page, tasks list and a blank starter page.
Authentication flows are also included: sign‑in, sign‑up, password reset and nicely styled 404/500 error pages.

Getting started

Because the dashboard is a static site, you can run it from your filesystem or from any HTTP server.
However, some JavaScript libraries expect an HTTP context; therefore, the recommended way to view the pages locally is to serve them via a simple development server:

# From within the project root
python3 -m http.server 8080

# or, if you have Node.js installed
npx http-server -p 8080


Once the server is running, open http://localhost:8080/DashboardTemplate/dashboard.html in your browser to see the dashboard page.
Navigate through the sidebar to explore the other pages.

Choosing a theme

The template ships with four stylesheets: modern, classic, dark and light.
By default, a small settings.js script reads the theme query parameter or a cookie to decide which stylesheet to load. For example:

dashboard.html?theme=dark will load css/dark.css instead of css/modern.css.

dashboard.html?theme=light will apply a lighter palette.

If no parameter or cookie is set, the modern theme is used.
You can also hard‑code a specific theme by editing the <link> tag in each HTML file (commented examples for each style are provided at the top of every page).

File structure
DashboardTemplate/
├── css/
│   └── modern.css           # Default Bootstrap‑based style (others: classic.css, dark.css, light.css)
├── dashboard.html           # Main dashboard page with charts, statistics and recent activity
├── forms‑*.html             # Demonstrations of basic, advanced, editor, validation and wizard forms
├── pages‑*.html             # Clients, invoice, pricing, tasks, settings and miscellaneous pages
├── pages‑sign‑*.html        # Sign in, sign up and password reset pages
├── pages‑404.html           # Custom 404 error page
├── pages‑500.html           # Custom 500 error page
├── js/
│   ├── app.js               # Bundled JavaScript for interactivity; includes jQuery, Bootstrap and plugins
│   └── settings.js          # Loads the appropriate CSS theme based on URL parameter or cookie
├── fonts/
│   └── *.woff2              # Font files for Font Awesome and Ion Icons
└── img/
    ├── avatars/             # User avatar images used throughout the templates
    └── photos/              # A few sample background photos

Customisation

The template is intended as a starting point. To adapt it for your own project:

Pick a theme by editing the <link> tag in the <head> of each page or by using the theme query parameter as described above.

Remove unused pages and modify the HTML to suit your application's needs. The sidebar navigation items can be edited in each file to point to your own routes.

Replace placeholder data (such as names, table rows and dashboard statistics) with real data from your backend.

Add or remove plugins by editing app.js. The bundled script imports jQuery plugins such as Select2, DateRangePicker, DataTables, Quill and ApexCharts. If you don't need a particular feature, remove its markup from the HTML and exclude the corresponding plugin script.

Localise text and change labels in the HTML as necessary.

The HTML is organised so that most components live inside Bootstrap cards and rows. Feel free to copy card markup into your own views and adjust colours and spacing via CSS.

Contributing

This template is provided as‑is for use in your own projects. If you find issues or wish to extend the functionality, feel free to fork the repository and make changes. There is no build system; simply edit the HTML, CSS and JavaScript files directly and test in your browser.

Licensing

The underlying libraries (Bootstrap, jQuery, Chart.js, ApexCharts, Select2, DataTables, etc.) are released under their respective open‑source licences.
The “Firma” design itself originates from Bootlab’s commercial admin template line. Ensure that you have the appropriate rights to use the template in your project and consult Bootlab’s licensing terms if necessary.
