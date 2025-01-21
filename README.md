Monsters Rolodex
============================

> Monsters Rolodex is a React-based application that allows users to search and filter a list of monsters. It demonstrates the use of React components, state management, lifecycle methods, and API integration.

### Overview

Monsters Rolodex is a React app that lets users search and filter a list of monsters. It fetches user data from `https://jsonplaceholder.typicode.com/users` and displays them as "monster cards." Each monster has a unique avatar generated using the URL: `https://robohash.org/${monster.id}?set=set4&size=180x180`.


### Folder Structure

    monsters-rolodex/
    ├── public/                  # Public assets (index.html, favicon, manifest.json)
    ├── src/                     # Source files
    │   ├── components/          # Reusable components
    │   │   ├── card/            # Card component
    │   │   │   ├── card.component.jsx
    │   │   │   └── card.styles.css
    │   │   ├── card-list/       # CardList component
    │   │   │   ├── card-list.component.jsx
    │   │   │   └── card-list.styles.css
    │   │   └── search-box/      # SearchBox component
    │   │       ├── search-box.component.jsx
    │   │       └── search-box.styles.css
    │   ├── App.css              # Main styles for the app
    │   ├── App.js               # Main React component
    │   ├── index.css            # Global styles
    │   ├── index.js             # ReactDOM render file
    │   └── reportWebVitals.js   # Performance metrics
    ├── .gitignore               # Git ignore file
    ├── package.json             # Project dependencies and scripts
    ├── README.md                # Project documentation
    └── yarn.lock                # Dependency lock file (if using Yarn)

### Setup Instructions

1. Clone the repository.
2. Install dependencies with `npm install`.
3. Start the app using `npm start`.
4. Access the app at `http://localhost:3000`.



### Components
- **App Component**: Main component managing state and rendering child components.
- **SearchBox Component**: Renders search input field to filter monsters.
- **CardList Component**: Maps over the list of monsters and renders a Card for each.
- **Card Component**: Displays monster details including name, email, and avatar.

  
### API Integration
- Fetches data from: `https://jsonplaceholder.typicode.com/users`.
- Each monster's avatar is generated dynamically using the following URL:
  - `https://robohash.org/${monster.id}?set=set4&size=180x180`
  - This generates a unique avatar for each monster based on their ID.