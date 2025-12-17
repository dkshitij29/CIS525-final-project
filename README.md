# CIS Final project

## CIS 525: AI-Powered Itinerary Generator

An intelligent application designed to generate personalized travel itineraries. This project utilizes a full-stack architecture with a React frontend, a Python backend, and a dedicated AI integration layer.

## 📂 Project Structure

The repository is organized into three main components:

  * **`cis525-frontend/`**: The client-side application built with React and Vite. It handles user authentication (Login/Signup) and itinerary display.

  * **`cis525_backend/`**: The server-side logic handling database connections, CRUD operations, and API requests.

  * **`CIS_525-AI_Powered_Itinerary_Generator/`**: The core AI logic, containing prompts and scripts for generating itineraries[cite: 1].

## 🚀 Technologies

  * **Frontend:** React, Vite, CSS.
  
  * **Backend:** Python, Database (likely PostgreSQL based on `db.config` and `crud.md.

  * **Deployment:** Render (indicated by `render.yml` and `render.yaml` configuration files).


## 🛠️ Installation & Setup

To run this project locally, you will need to set up each service individually.

### Prerequisites

  * Node.js and npm
  * Python >= 3.10 and < 3.13
  * pip

### 1\. Backend Setup (`cis525_backend`)

1.  Navigate to the backend directory:
    ```bash
    cd cis525_backend
    ```
2.  Install dependencies:
    ```bash
    pip install -r requirements.txt
    ```
3.  Configure the database:
      * Review `db/db.config` and `db/db.md` for connection details[cite: 1].
4.  Run the application:
    ```bash
    cd src
    uvicorn main:app --reload
    ```
      * *Note: There is also a shell script available at `src/testmain.sh` for testing execution.*

### 2\. Frontend Setup (`cis525-frontend`)

1.  Navigate to the frontend directory:
    ```bash
    cd cis525-frontend
    ```
2.  Install dependencies:
    ```bash
    npm install
    ```
3.  Start the development server:
    ```bash
    npm run dev
    ```
      * This uses Vite to serve the app locally.

### 3\. AI Service Setup (`CIS_525-AI_Powered_Itinerary_Generator`)

1.  Navigate to the AI service directory:
    ```bash
    cd CIS_525-AI_Powered_Itinerary_Generator
    ```
2.  Install requirements:
    ```bash
    pip install -r requirements.txt
    ```
3.  Run the generator:
    ```bash
    cd src
    uvicorn main:app --reload
    ```

## ✨ Key Features

  * **User Authentication:** Includes dedicated pages for Login (`LoginPage.jsx`) and Sign Up (`SignUpPage.jsx`).
  * **Itinerary Management:** Users can input travel details via `Form.jsx` and view generated plans on the `ItineraryListPage.jsx.
  * **AI Integration:** Utilizes custom prompts (`prompt.txt`) to generate tailored travel schedules.

## ☁️ Deployment

This project is configured for deployment on **Render**.

  * Configuration files: `render.yml` (in the AI folder) and `render.yaml` (in the Backend folder).
  * The setup suggests a microservices approach where the backend and the AI generator may be deployed as separate services.

## 📝 Database

Database documentation and CRUD operation guides are located in `cis525_backend/db/`:

  * `db.md`: General database documentation[cite: 1].
  * `crud.md`: Specifics on Create, Read, Update, Delete operations.

## 🤝 Contributing

1.  Fork the repository.
2.  Create a feature branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

-----

**Note:** This project is part of the CIS 525 coursework.
**Disclaimer**: The project API keys are shut down by the admin. Due to increased OPEX.

-----
