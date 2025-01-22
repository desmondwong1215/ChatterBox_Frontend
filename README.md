# ChatterBox Frontend

Welcome to the **ChatterBox Frontend** repository! This is the frontend implementation of ChatterBox, a modern forum application that enables users to discuss and share ideas. The project is built using **React** and **Vite** and communicates with a backend API hosted on Render.

## Table of Contents
- [Features](#features)
- [Technologies Used](#technology-used)
- [Getting Started](#getting-started)
- [Running Locally](#running-locally)
- [Deployment](#deployment)
- [Contributing](#contributing)
- [Troubleshooting](#troubleshooting)
- [Contact](#contact)

## Features
- User Authentication (Login and Signup)
- Persistent Login using JWT and Cookies
- Create, Read, Update, and Delete (CRUD) forum posts
- Responsive Design for mobile and desktop
- Error handling for seamless user experience

## Technologies Used
- **React**: JavaScript library for building user interfaces.
- **Vite**: A fast and modern development build tool.
- **Axios**: For making HTTP requests to the backend.
- **React Router**: For managing client-side routing.
- **CSS**: For styling and responsiveness.

## Getting Started
This website is live at [ChatterBox](https://my-chatterbox.netlify.app). For more information, refer to `/UserManual.txt`.

### Prerequisites
Before you begin, ensure you have the following installed on your system:
- [Node.js](https://nodejs.org/): v16+ recommended
- [npm](https://www.npmjs.com/) or [yarn](https://yarnpkg.com/): Node package manager
- [ChatterBox_Backend](https://github.com/desmondwong1215/ChatterBox_Backend): Backend Api

### Installation
1. Clone the repository:
   ```bash
   git clone https://github.com/desmondwong1215/ChatterBox-Frontend.git
   ```

2. Navigate to the project directory:
   ```bash
   cd ChatterBox-Frontend
   ```

3. Install dependencies:
   ```bash
   npm install
   # or
   yarn install
   ```

## Running Locally
1. Install [ChatterBox_Backend](https://github.com/desmondwong1215/ChatterBox_Backend) to run ChatterBox backend locally. In `src/forumAxios.tsx`, comment out line 4 and uncomment line 7.

3. Start the development server:
   ```bash
   npm run dev
   # or
   yarn dev
   ```

3. Open your browser and navigate to `http://localhost:5173` to view the app.

## Deployment
This project can be deployed to **Netlify** or any other static hosting provider.

### Deploying to Netlify
1. Push your repository to GitHub.
2. Log in to [Netlify](https://www.netlify.com/) and create a new site.
3. Connect your GitHub repository.
4. Set the build settings:
   - **Build Command**: `npm run build`
   - **Publish Directory**: `dist`
5. Create a `public` directory if it does not exist, add an `_redirects` file in the `public/` directory to handle single-page application routing:
   ```
   /* /index.html 200
   ```
6. Deploy the site. Your application will be live at the Netlify URL provided.

## Troubleshooting
1. CORS Issues
If you encounter CORS issues when connecting to the backend, ensure that the backend has proper CORS settings configured.

2. Page Redirects to Login
If cookies or local storage items disappear on reload:
   - Check the domain and path settings for cookies.
   - Verify the backend correctly sets `SameSite` and `Secure` attributes.

## Contributing
Contributions are welcome! If you have ideas for improvements or encounter any issues, feel free to open an issue or submit a pull request.

### Steps to Contribute
1. Fork the repository.
2. Create a new branch:
   ```bash
   git checkout -b your-feature-name
   ```
3. Make your changes and commit them:
   ```bash
   git commit -m "Add your feature"
   ```
4. Push the branch to your fork:
   ```bash
   git push origin your-feature-name
   ```
5. Open a pull request to the `main` branch.

## Contact
1. For any inquiries or support, please contact:
   - **Name**: Desmond Wong Hui Sheng
   - **Email**: e1356940@u.nus.edu
   - **GitHub**: https://github.com/desmondwong1215

---
Feel free to explore, contribute, and build something amazing with ChatterBox!
