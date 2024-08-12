# Todo Project Manager

This repository serves as the umbrella for the full-stack Todo Project Manager application, which is divided into two separate repositories:

## 📂 Repositories

### Frontend
- **Technology**: Angular
- **Repository**: [Frontend Repository](https://github.com/ashishs1460/ProjectTodoManager-Frontend.git)

### Backend
- **Technology**: Spring Boot
- **Repository**: [Backend Repository](https://github.com/ashishs1460/ProjectTodoManager-Backend.git)

## 📊 Database Design
![Database Design](ToDo_DB_Design.png)

## 🌐 Live Demo
You can view the live demo of the project here: [Live Demo](https://project-todo-manager-frontend.vercel.app/)

## 📹 Demo Video
Check out this video: [Demo Video](https://www.youtube.com/watch?v=A4_44Nd82wM)

## 🛠️ Setup Instructions to Run Locally

### Frontend

1. **Clone the Frontend Repository**:  

2. **Update URLs**:  
- Replace the URLs in `http-token-interceptor` with your localhost URL.
- Update the URL in `GistService` (`backendOAuthUrl`) with your local backend URL.
- Inside the `getGithubToken` method, replace the `redirectUri` with your frontend local URL.
- In `ProductDetailsComponent`, update the `redirectUri` in the `exportAsGist()` method with your frontend local URL.

3. **Set Up GitHub OAuth**:  
- Go to GitHub Developer Settings and create a new OAuth App.
- Generate a Client ID and Client Secret.
- Use these credentials in the backend `application.yaml` file.

4. **Install Dependencies & Run**:  
- Navigate to the project directory and run:
`npm install`
`ng serve`
- The frontend application will be up and running.

### Backend

1. **Clone the Backend Repository**:  

2. **Execute SQL Script**:  
- Navigate to `src/main/resources/sql`.
- Execute the `todo.sql` script using your preferred database workbench.

3. **Update Database Configuration**:  
- In the `application.yaml` file, update the database configuration with your local database details.

4. **Configure CORS**:  
- In the `SecurityConfig` class (within the `configuration` package), update the CORS configuration with your frontend local URL.

5. **Run the Backend Application**:  
