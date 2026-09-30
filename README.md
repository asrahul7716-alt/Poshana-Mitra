# Poshana Mitra - Diet & Nutrition Awareness Tool

A free, watermark-free website for tracking children's nutrition and suggesting balanced meal plans for anganwadi children under nutrition schemes.

## Features

- **Bilingual Support**: English and Kannada language toggle
- **User Authentication**: Login/logout system (client-side storage for demo)
- **Meal Tracking**: Log daily meals for children by food type and time
- **Meal Planner**: Generate balanced weekly meal plans based on age and nutritional guidelines
- **Dashboard**: Overview of nutritional intake, status, and upcoming meal plans
- **Responsive Design**: Works on mobile and desktop devices
- **Offline Functionality**: Works offline once loaded (uses localStorage)
- **Free Hosting**: Can be hosted for free on GitHub Pages (no watermarks)

## Technology Stack

- **Frontend**: HTML5, CSS3, Vanilla JavaScript
- **Storage**: browser localStorage for persistence
- **Hosting**: GitHub Pages (or any static site host)
- **Meal Planning Logic**: Ported from the existing Python meal planner (rule-based algorithm)

## Project Structure

```
diet-nutrition-website/
├── index.html          # Landing page/login page
├── dashboard.html      # Main dashboard after login
├── meal-planner.html   # Meal planning interface
├── track-meals.html    # Meal tracking interface
├── css/
│   ├── styles.css      # Main stylesheet (uses CSS variables)
│   ├── responsive.css  # Responsive design adjustments
│   └── theme.css       # Theme variables (light/dark)
├── js/
│   ├── storage.js      # localStorage utility functions
│   ├── auth.js         # Authentication handling (login/logout)
│   ├── language.js     # Language translation and toggle
│   ├── main.js         # Core application logic
│   ├── meal-planner.js # Meal planning logic (ported from Python)
│   ├── track-meals.js  # Meal tracking logic
│   ├── dashboard.js    # Dashboard logic
│   └── init.js         # Initialize demo data if none exists
├── lang/
│   ├── en.json         # English translations
│   └── kn.json         # Kannada translations
├── data/
│   ├── food_data.json  # Nutritional food database (from existing project)
│   └── schema.sql      # Database schema (for reference, optional)
├── assets/
│   ├── icons/          # SVG icons
│   └── images/         # Logo and illustrations
└── README.md           # This file
```

## How to Run Locally

1. Clone or download this repository to your local machine.
2. Open `index.html` in your web browser (Chrome, Firefox, Safari, or Edge).
3. The site should load and you can start using it.

Note: For the best experience, use a modern browser with localStorage support.

## Deployment to GitHub Pages (Free)

1. Create a GitHub account (if you don't have one).
2. Create a new public repository (e.g., `poshana-mitra`).
3. Clone the repository locally or upload the files via GitHub's web interface.
4. Ensure all files are in the root of the repository (no subdirectory for the site).
5. Go to repository Settings > Pages.
6. Under "Source", select the `main` branch and `/` (root) folder.
7. Click "Save". GitHub will publish your site.
8. Your site will be available at `https://<username>.github.io/<repository-name>/`.

## Demo Credentials (if initialized)

If the site finds no existing users, it will create a demo user:
- Username: `demo`
- Password: `demo123`

## Name Suggestions

The website is named "Poshana Mitra" (Poshana = nutrition in Sanskrit, Mitra = friend). Other suggestions included:
- Arogya Mitra
- Srushti Poshan
- Balanced Bites
- Swasta Mane
- Poshana Tracker
- Ankur Poshan
- Susthir Poshan

## Future Enhancements

- Add data export/import functionality
- Implement anonymous usage analytics (opt-in)
- Add offline-first capabilities with service workers
- Integrate with government nutrition APIs (if available)
- Add multi-child tracking for families
- Implement gamification elements to engage children
- Add voice input for accessibility

## Acknowledgments

This project leverages the existing Diet & Nutrition Awareness Tool for Anganwadi Children project (found in Downloads/SendAnywhere_756612) for its food data schema and meal planning logic.

---
*Built as a free, watermark-free solution for Diet & Nutrition awareness targeting anganwadi children.*