# LoanSwiftPro

<!-- PROJECT LOGO -->

<div align="center">
  <a href="https://github.com/BhagyaRana/LoanSwiftPro">
    <img src="/frontend/src/assets/lsp-logo-transparent.png" height="150" alt="LoanSwiftPro-Logo">
  </a>
  <h3 align="center">LoanSwiftPro</h3>
  <p align="center">
    Your Fastlane to Financial Freedom
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#project-overview">Project Overview</a>
    </li>
    <li>
      <a href="#project-components">Project Components</a>
    </li>
    <li>
      <a href="tech-stack">Tech Stack</a>
    </li>
    <li>
      <a href="#project-architecture">Project Architecture</a>
    </li>
    <li>
      <a href="#prerequisites">Prerequisites</a>
    </li>
    <li>
      <a href="#installation">Installation</a>
    </li>
    <li>
      <a href="#demo">Demo</a>
    </li>
    <li>
      <a href="#usage">Usage</a>
    </li>
    <li>
      <a href="#use-case-diagram">Use Case Diagram</a>
    </li>
    <li>
      <a href="#challenges-faced">Challenges Faced</a>
    </li>
    <li>
      <a href="#future-scope">Future Scope</a>
    </li>
    <li>
      <a href="#team-members">Team Members</a>
    </li>
    <li>
      <a href="#contributing">Contributing</a>
    </li>
    <li>
      <a href="#license">License</a>
    </li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->

## Project Overview

LoanSwift Pro is a comprehensive Loan Management Application designed to simplify and streamline the loan application process for users. It leverages modern web technologies to provide a seamless experience for both applicants (LUMA) and administrators (LAMA).

Key Features

1. **User-Friendly Interface**: Intuitive and Responsive UI, ensuring a seamless experience for users.

2. **Multi-Loan Support**: Users can apply for various types of loans, such as personal loans, mortgages, or car loans, all within a single platform.

3. **Loan Application Tracking**: Applicants can track the status of their loan applications in real-time, reducing the need for follow-up communication.

4. **Administrative Dashboard**: Admins have access to a powerful dashboard for managing user accounts, reviewing applications, and generating reports

5. **Secure Authentication**: Robust user authentication and authorization mechanisms ensure data security and privacy.

<!-- PROJECT COMPONENTS -->

## Project Components

<div align="center">
  <img src="/frontend/public/components.PNG" alt="project-components">
</div>

<!-- ABOUT THE PROJECT -->

## Tech Stack

<div align="center">
  <img src="/frontend/public/tech_stack.PNG" alt="tech-stack">
</div>

## Project Architecture

<div align="center">
  <img src="/frontend/public/three-tier-architecture.PNG" alt="architecture-1">
</div>
<br />
<div align="center">
  <img src="/frontend/public/architecture.PNG" alt="architecture-2">
</div>

<!-- PREREQUISITES -->

## Prerequisites

Before you begin, make sure you have the following prerequisites installed on your system:

- **Node.js and npm**: Required for running the frontend.
- **Java**: Required for running Spring Boot.
- **MySQL**: Required for the database.

<!-- INSTALLATION -->

## Installation

<details>

<summary>Step 1 : Clone the Repository </summary>
<p>
First, clone the project repository to your local machine using the following command:

```

git clone https://github.com/BhagyaRana/LoanSwiftPro.git

```

</p>

</details>

<details>

<summary>Step 2 : Set Up the Database </summary>
<p>

Open a MySQL client and create a new database ('loan') for this project.

```

create database loan; use loan;

```

In the project's backend directory, locate the application.properties file (usually found in the src/main/resources directory).

Update the 'application.properties' file with your database configuration. Replace the following placeholders with your database details:

```

spring.datasource.url=jdbc:mysql://localhost:3306/loan
spring.datasource.username=your-database-username
spring.datasource.password=your-database-password

```

Save the application.properties file.

</p>
</details>

<details>
  <summary>Step 3 : Set Up the Backend</summary> 
  <p>Open a terminal and navigate to the project's backend directory:

`cd your-project/backend`

Build the Spring Boot project using Maven:

`mvn clean install`

Start the Spring Boot application:

`java -jar target/your-project-backend.jar`

The backend should now be running on http://localhost:8080.

Alternatively, you can open the `backend` folder in Ecclipse / IntelliJ and Run `LoanAppApplication.java` located at `backend/src/main/java/com/training/loan_app/LoanAppApplication.java`.</p>

</details>

<details>
  <summary>Step 4 :  Set Up the Frontend</summary> 
  <p>
  Open a new terminal and navigate to the project's frontend directory:

`cd your-project/frontend`

Install the frontend dependencies:

`npm install`

Start the React development server:

`npm start`

The frontend should now be running on http://localhost:3000.</p>

</details>

<details>
  <summary>Step 5 : Access the Application</summary> 
  <p>You can now access the application in your web browser. Open your browser and navigate to http://localhost:3000 to interact with the React frontend.

Your Spring Boot backend is running on http://localhost:8080 and is ready to handle API requests from the frontend.

You have successfully set up and run the project with MySQL, Spring Boot, and React. You can now start developing and using your application.</p>

</details>

<!-- DEMO -->

## Demo

<!-- TODO: Add Project Deployment Link -->

You can see a live demo of our project <a href="#">here</a>.

<!-- USAGE -->

## Usage

1. Register New User / Admin.
2. Login via Credentials
3. Admin need to Add which all Loans that Customer can Avail from Dashboard
4. User can check which all loans are available and Apply for it
5. User and Admin can view Loan Purchase History and admin has Rights to Modify it as well.

<!-- USE CASE -->

## Use Case Diagram

<div align="center">
  <img src="/frontend/public/use-case-diagram.PNG" alt="use-case-diagram">
</div>

<!-- CHALLENGES -->

## Challenges Faced

- **Integration**: Making React and Spring work together smoothly can be tricky.

- **Security**: Safeguarding user data and ensuring secure access requires careful handling.

- **State Management**: Managing data across React components can get complex.

- **Performance**: Ensuring the app runs fast, even with lots of users, can be a challenge.

- **Scalability**: Designing the app to handle growth in users and data can be tough

- **User Experience**: Creating an easy-to-use interface for applying for loans is important but can be hard.

- **Concurrency**: Handling multiple users doing things at the same time is tricky.

- **Cross-Browser Compatibility**: Making the app work well in different web browsers can be challenging.

<!-- FUTURE SCOPE -->

## Future Scope

- **Loan Repayment Calculators**: Users can estimate their monthly loan payments, helping them make informed decisions. We are Currently just Applying for Loan and not Calculating the Financing Aspects like EMI.

- **Increased Security**: Implementing Spring Security with Combination of JWT and OAuth.

- **Integration with External Services**: The application leverages Axios to connect with external services for credit scoring, document verification, and more.

- **Deployment**: Docker containers for application and database, Nginx as a reverse proxy, AWS (or your preferred cloud provider) for hosting.

- **Mobile App**: Developing a mobile app version to provide users with on-the-go access.

- **Notifications**: Implementing email or SMS notifications for application status updates.

- **Credit Score Integration**: Integrating with credit bureaus for real-time credit scoring.

- **Document Upload**: Allowing users to upload documents directly through the application & using OCR + AI for calculating Eligible Credit Amount.

<!-- TEAM MEMBERS -->

## Team Members

- Bhagya Rana - <a href = "https://github.com/BhagyaRana/">@Bhagya</a>
- Puttaraja Hosalli- <a href = "https://github.com/Puttaraja">@Puttaraja</a>
- Akash Bose - <a href = "https://github.com/akashhhhhb">@Akash</a>
- Anshuman Singh - <a href = "https://github.com/anshuman924">@Anshuman</a>
- Anjali Kumari - <a href = "https://github.com/AnjaliChaubey19">@Anjali</a>

<!-- CONTRIBUTING -->

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

<!-- LICENSE -->

## License

Distributed under the MIT License. See `LICENSE.txt` for more information.
