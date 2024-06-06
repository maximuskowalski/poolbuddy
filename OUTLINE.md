# Purpose

**Poolbuddy** is designed to streamline the management of pool data and chemical balances for pool operators. The application aims to facilitate the efficient monitoring, recording, and analysis of pool conditions, ensuring optimal operational standards and safety.

## Goals

1. **Comprehensive Data Management**:
    - **Data Collection**: Enable users to input and store various pool measurements such as pH levels, chlorine content, temperature, and more.
    - **Data Accessibility**: Provide quick access to the latest pool measurements and allow users to view historical data for long-term trends and analytics.

2. **Enhanced Monitoring and Reporting**:
    - **Real-Time Monitoring**: Allow users to check the current state of the pool and view the latest values at any time.
    - **Trend Analysis and Reporting**: Help users identify ongoing issues through analytics that highlight trends and changes over time.

3. **Collaborative Features**:
    - **User Notes**: Enable users to view and share notes on specific pools, fostering better communication and information sharing among team members or across different user roles.
    - **Shared Access**: Ensure that measurements and reports can be easily accessed by all relevant parties, enhancing teamwork and management efficiency.

4. **Inventory Management**:
    - **Stock Tracking**: Include features for tracking the stock levels of chemicals, equipment, and spare parts, aiding in inventory control and planning.

5. **Proactive Maintenance and Correction**:
    - **Automated Calculations**: Provide automated chemical correction suggestions based on the latest measurements and predefined pool parameters (e.g., volume, turnover rate).
    - **Correction Reminders**: Offer reminders for re-testing water quality after chemical corrections or at regular intervals (e.g., every four hours during public opening times) to maintain pool standards.

6. **User-Centric Design**:
    - **Ease of Use**: Develop an interface that is intuitive and easy to navigate, enabling users to perform tasks efficiently and without extensive training.

## Key Features

- **User Authentication**: Secure login/logout, password recovery, and user registration.
- **Data Input**: Interface for entering pool readings like pH, chlorine levels, temperature, etc.
- **Data Visualization**: Dashboard to display historical data and trends over time.
- **Analytics and Reporting**: Generate reports based on specified criteria (e.g., date ranges).
- **Chemistry Correction Advice**: Algorithms to suggest chemical adjustments based on pool readings.
- **Sharing and Collaboration**: Ability for users to share pool data with others, such as team members or other departments.
- **Alerts and Notifications**: Implement real-time alerts for critical readings or when scheduled tasks (e.g., testing, maintenance) are due. This can enhance responsiveness and preventive maintenance.
- **Multi-language Support**: For users from non-English-speaking regions, offering multiple languages.
- **Inventory Management**: Integrate an inventory management system for chemicals and equipment. This feature can help in predicting when supplies are low and need reordering.
- **Mobile Optimization**: Ensure all features are fully functional on mobile devices, considering that users might access the app in various environments, especially while physically at the pool site.
- **Customizable Access Levels**: Allow more granular control over what each user role can view, edit, or delete. This can help in managing large teams with diverse responsibilities.

## User Roles

- **Administrator**: Manages user accounts, access permissions, and can view/edit all entries.
- **Company Manger:** Can manage all facilities and pools within the company, assign user roles and access permissions within that company.
- **Facility Manager:** Can manage all pools and users within that facility, assign user roles and access permissions within that facility. Oversee multiple pools, can add/remove pools, view reports, and manage data for their specific pools.
- **Standard User**: Can input data, view statistics of pools they have access to, and receive suggestions for chemical adjustments. Send current information to manager to request assistance.
- **Restricted User**: Can view statistics of pools they have access to
- **Guest User**: Might be useful for temporary or trial access, allowing potential customers to explore the app with limited capabilities before committing.
- **Technical Support**: Role for users who handle technical issues and assist other users with troubleshooting problems within the app.

## User Journeys

- **Sign Up/Sign In**: Process for user registration and login, including handling forgotten passwords. Membership, request membership of pool, facility, company.
- **Entering Data**: Steps a user follows to input new pool readings. Comments and notes. Photos?
- **Viewing Reports**: How users access and interact with historical data.
- **Receiving Recommendations**: How the system provides chemical adjustment advice based on the latest data.
- **Inventory Management**: Journey for managing inventory (adding new stock, updating existing stock, viewing stock levels). Particularly useful for facility managers and administrators.
- **Alerts Response**: Path that a user would follow upon receiving an alert, including steps for acknowledging the alert, taking corrective actions, and logging these actions.
- **Custom Report Generation**: Allow users to create custom reports by selecting specific data points, date ranges, and visual representations. This could be particularly useful for managers during reviews or planning.
- **Profile Management**: Journey for users to manage their profiles, including updating contact information, changing passwords, and setting preferences.

## Additional Considerations

- **API Integrations**: If there's potential to integrate with other systems (e.g., automated pool maintenance systems), consider developing an API that allows for such integrations.
- **Feedback Mechanism**: Include a way for users to provide feedback directly within the app. This can be crucial for continuous improvement and user satisfaction.

## Priority of Features

### MUST HAVE

These are essential features that the app needs to function effectively from day one. They are non-negotiable as they form the backbone of the app's functionality.

- **User Authentication**: Secure login, logout, and registration processes to ensure user data is protected and access is controlled.
- **Data Input**: Interface for entering essential pool readings (pH, chlorine levels, temperature, etc.). This is critical for the core functionality of recording and managing pool data.
- **Data Visualization**: Basic dashboard to display current and historical data. This is essential for users to make sense of the data they input.
- **Chemistry Correction Advice**: Core algorithms to suggest chemical adjustments based on pool readings. This is a key selling point and necessary for the app's value proposition.

### SHOULD HAVE

Important features that enhance user experience and functionality but are not immediately critical for the app's operation. These features can be developed after the initial core features are stable.

- **Analytics and Reporting**: Advanced analytical tools and customizable reports based on specified criteria (e.g., date ranges). While important for deeper insights, the app can function at a basic level without them initially.
- **Sharing and Collaboration**: Features that allow users to share pool data and notes with others. Essential for teamwork but can be enhanced over time.
- **Alerts and Notifications**: To inform users about critical conditions or when specific tasks are due. Enhances user engagement and proactive management.
- **Inventory Management**: Basic tracking of chemicals and equipment stock levels. Important for operational efficiency but can initially be handled manually if necessary.

### COULD HAVE

These are desirable features that can significantly improve user satisfaction and operational efficiency but are not essential for the initial launch.

- **Multi-language Support**: Expands the app’s usability across different regions but is not critical for initial launch.
- **Customizable Access Levels**: Allows detailed control over what each user role can access. While beneficial, the initial release can operate with fixed role permissions.
- **Mobile Optimization**: Although the app should be responsive from the start, full optimization for mobile devices can be refined post-launch.

### WONT HAVE

Features that are outside the scope of the initial release but may be considered for future updates based on user feedback and market demands.

- **API Integrations**: Potential future enhancements to integrate with other systems or platforms. Not necessary for initial functionality.
- **Guest User Role**: While useful for promotional purposes, creating a trial or demo mode is not critical for the initial launch.
- **Advanced Custom Report Generation**: Highly customizable reports are a great feature for power users but can be developed after gathering user feedback on basic reporting needs.

## Technical and Non-Technical Requirements

### Technical Requirements

- **Frontend Technologies**:

  - **SvelteKit**: Used for building a dynamic and responsive user interface. It offers a simpler developer experience and less boilerplate than React or Vue.js, making it a great choice for beginners.
  - **Tailwind CSS**: For responsive design to ensure the app looks good on both desktop and mobile devices. Tailwind provides utility-first CSS that is highly customizable and easy to maintain.

- **Backend Technologies**:

  - **PocketBase**: Serves as an all-in-one backend solution that includes a database, real-time data capabilities, and built-in user authentication. It simplifies many backend development tasks and can be used to serve static files for SvelteKit, making it ideal for small to medium projects.

- **Database**:

  - **PocketBase uses SQLite**: This is integrated into PocketBase and simplifies data management, eliminating the need for separate database setup and maintenance.

- **Authentication**:

  - **Built-in with PocketBase**: PocketBase provides built-in authentication mechanisms that are simple to set up and include features necessary for secure logins, password recovery, and user management.

- **Data Analysis and Reporting**:

  - **Python (Optional)**: For sophisticated data analysis and reporting needs that might arise later. Python can be integrated as a separate microservice or run scripts on-demand to process data and generate reports. This setup allows you to use Python's powerful libraries like Pandas and Matplotlib.

- **APIs**:

  - **RESTful API Design**: Although PocketBase handles most backend interactions, additional custom APIs can be developed if needed using lightweight frameworks like Flask in Python, especially for complex data operations not covered by PocketBase.

- **Development and Deployment Tools**:

  - **Docker**: For containerizing the application, ensuring consistency across different environments and simplifying deployment processes.
  - **GitHub**: For version control and as a platform for using CI/CD workflows to automate deployment processes.

- **Security Requirements**:

  - **HTTPS**: To secure data in transit.
  - **Data Encryption**: At rest and in transit, especially sensitive user and pool data.
  - **Regular Security Audits**: To ensure vulnerabilities are identified and mitigated.

- **Compliance and Data Handling**:

  - **GDPR Compliance**: If operating in or handling data from the European Union.
  - **Data Backup and Recovery**: Strategies to prevent data loss and ensure continuity.

### Non-Technical Requirements

1. **Usability**:

    - **Intuitive User Interface**: Easy navigation and minimalistic design to enhance user experience.
    - **Onboarding Process**: Guided tours or help sections for new users to understand the app’s features quickly.

1. **Accessibility**:

    - **ADA Compliance**: Ensure the app is accessible to users with disabilities, including screen reader compatibility and keyboard navigability.
    - **Responsive Design**: The app should be fully functional on both desktop and mobile devices.

1. **Legal and Regulatory Considerations**:

    - **Privacy Policy and User Agreement**: Clearly defined terms of use and privacy policy that comply with local and international laws.
    - **Chemical Handling and Reporting Regulations**: Compliance with local health and safety standards regarding pool management.

1. **Support and Documentation**:

    - **User Manuals**: Comprehensive guides on how to use the app.
    - **Technical Support**: Dedicated support channels for users experiencing issues.

1. **Marketing and User Adoption**:

    - **Marketing Strategies**: Plans to promote the app through various channels.
    - **Feedback Mechanisms**: Features allowing users to give feedback to continuously improve the app.

This structured approach ensures that all aspects of the app's development are considered, from technical implementation to user experience and compliance. Each category should be reviewed and updated as the project progresses and as more information becomes available

## Feedback and Validation

- **Stakeholder Review**: Present plan to stakeholders or potential users for feedback.
- **Adjustments**: Refine your requirements based on the feedback received.

## Documentation

- Create detailed documentation of all the requirements. This document will guide the development process and help ensure that nothing important is overlooked.

## Other

 It might also be beneficial to create visual diagrams like flowcharts or wireframes during this phase to visualize the user journeys and data flow.

### Suggestions for Enhancement

- **Mobile Optimisation**: Ensure that the app is fully optimised for mobile use, allowing pool managers and staff to input and access data on the go.
- **Alerts and Notifications**: Implement alerts for critical conditions or when measurements fall outside safe parameters, prompting immediate attention.
- **Customisable Reports**: Allow users to customise reports based on specific data points, time frames, and formats to meet diverse operational needs.
