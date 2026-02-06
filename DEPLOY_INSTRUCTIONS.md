# How to Deploy to Netlify (Recommended)

This guide will help you deploy your WhatsApp Chat Intelligence app to a public URL using Netlify and GitHub. This is the professional way to deploy, allowing your site to update automatically whenever you save changes.

## Prerequisites
- A GitHub account.
- A Netlify account (you can sign up with GitHub).

## Step 1: Push Your Code to GitHub
1.  Open your terminal/command prompt in this project folder.
2.  Run the following commands one by one:

    ```bash
    git add .
    git commit -m "Prepare for Netlify deployment"
    # If you haven't linked a repo yet, create one on GitHub first, then run:
    # git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
    git branch -M main
    git push -u origin main
    ```

## Step 2: Deploy on Netlify
1.  Log in to [Netlify](https://app.netlify.com/).
2.  Click **"Add new site"** > **"Import an existing project"**.
3.  Select **GitHub**.
4.  Authorize Netlify to access your GitHub repositories.
5.  Search for and select your repository (`whatsapp-chat-intelligence` or whatever you named it).
6.  **Build Settings**:
    -   **Base directory**: (Leave empty)
    -   **Build command**: (Leave empty)
    -   **Publish directory**: `.` (Netlify should detect this from `netlify.toml`, but verify it ensures it's just a dot `.` or cleared out if it defaults to something else, referencing the root).
7.  Click **"Deploy site"**.

## Step 3: Success!
- Netlify will generate a URL for you (e.g., `https://your-site-name.netlify.app`).
- You can change the site name in **Site settings** > **Change site name**.

