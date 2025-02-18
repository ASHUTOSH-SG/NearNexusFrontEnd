## NearNexus-FrontEnd

This project is a front-end website developed using React, HTML, CSS, and JavaScript. It serves as an interactive platform to showcase and explore a variety of electronic products. The product data is fetched from the (https://jsonkeeper.com/b/2XS9), which provides a comprehensive list of electronic items.

## Installation

To run this project locally, follow these steps:

1. Clone the repository to your local machine:

    ```
    git clone https://github.com/your-username/your-repository.git
    ```

2. Navigate to the project directory:

    ```
    cd your-repository
    ```

3. Install the required Node modules:

    ```
    npm install
    ```

## Build

To prepare the project for deployment, use the following command:

    ```
    npm build
    ```

This command optimizes and bundles the project files, making it deployment-ready.

## Running the App

To start the application on your local machine, use the following command:

    ```
    npm start
    ```

This will launch the app on your localhost, and you can access it through your web browser.

## Product Data API

The electronic product data is sourced from the (https://jsonkeeper.com/b/2XS9).  enabling the seamless integration of product listings into our project.

---

## **Deployment of NearNexusFrontEnd-REACT on AWS**

This document describes the deployment process for the **NearNexusFrontEnd-REACT** project on Amazon Web Services (AWS) using S3 for static website hosting.

### **Deployment Steps done**

#### **1. Set up S3 Bucket for Static Hosting**
The first step in deploying the React app was to create an **S3 bucket**. This is the storage location where the built React app will be uploaded. The following actions were performed:
- **S3 Bucket Creation**: A new S3 bucket was created with a globally unique name. This bucket was set to a public access configuration to allow public traffic to the app.
- **Static Website Hosting**: After creating the S3 bucket, **static website hosting** was enabled in the S3 properties section. This feature allows S3 to serve the React app as a static website, where:
  - The **index.html** file is specified as the entry point of the app.
  - Public access permissions were configured to make the files accessible via a URL.

#### **2. Build the React Application**
To prepare the React application for deployment:
- The `npm run build` command was executed to create a production-ready version of the app. This command compiles the React code into static files (HTML, CSS, JavaScript) that can be served by a web server.
- The output of this command is the **build/** directory, which contains all necessary assets for the application to run on any web browser.

#### **3. Upload the Build Files to S3**
After building the app, the next step was to upload the **build/** directory files to the S3 bucket:
- All the static files (including HTML, JavaScript, and CSS files) from the `build/` directory were uploaded to the S3 bucket.
- The S3 console was used for this purpose, where the files were selected and uploaded directly to the bucket.

#### **4. Access the Application**
Once the files were uploaded:
- The app was made publicly accessible via the **S3 static website hosting URL**.
- The website URL provided by AWS S3 allows the application to be accessed directly via the browser.

### **Outcome**
After completing the above steps, the **NearNexusFrontEnd-REACT** application was successfully deployed and made available for public access on AWS S3 as a static website.

---



