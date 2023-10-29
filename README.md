# Google Auth React Demo

This guide provides step-by-step instructions on how to integrate Google authentication into your application.

## Step 1: Create a react application using vite

```
npm create vite@latest
npm install
```

## Step 2: Install Required Package

To integrate Google authentication into your application, begin by installing the `@react-oauth/google` package. This package is Google's Identity Services SDK, which enables seamless integration of Google login into your application and facilitates secure access to Google APIs.

## Step 3: Acquire a Google Client ID

A client ID is essential for OAuth 2.0 authentication between the client and server. To obtain a Google Client ID, follow these steps:

1. Go to your Google Cloud Console.

2. Create a new project and name it according to your preference.

3. Select your project from the dashboard.

## Step 4: Create a Web Client ID

To create your web client ID, follow these steps in your project's Google Cloud Console:

1. Click on the "Credentials" tab in the left-side menu.

2. Click on "CREATE CREDENTIALS" at the top of the page.

3. Choose the "OAuth client ID" option.

4. Select "Web application" as the application type if you are integrating it into a React app.

5. Name your client ID descriptively, e.g., "Web ID."

6. Add the following URLs:
   - **Authorized JavaScript Origins**: URLs from which your application originates the login (e.g., localhost, localhost:3000 for React developers, or your hosted URL).
   - **Authorized Redirect URLs**: The URL Google will redirect the user to after a successful login.

   Example for localhost:
   - **Authorized JavaScript Origins**: http://localhost:3000
   - **Authorized Redirect URLs**: http://localhost

7. Click the "Create" button to generate your web client ID.

8. Copy your newly created web client ID from the dashboard.

## Step 5: Integration

Now that you have your web client ID, you can proceed to integrate Google login into your React app using the acquired credentials.

## Step 6: Run the app

```
npm run dev
```

Happy coding and enjoy the benefits of Google authentication in your application! 🚀🔑

