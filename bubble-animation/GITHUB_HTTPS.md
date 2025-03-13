# Using HTTPS for GitHub

To clone and push to your repository using HTTPS:

1. Create your repository on GitHub if you haven't already

2. Clone your repository using HTTPS:
   ```bash
   git clone https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
   ```

3. Navigate to your local repository:
   ```bash
   cd YOUR_REPO_NAME
   ```

4. Copy your files to this directory

5. Add the files:
   ```bash
   git add .
   ```

6. Commit the changes:
   ```bash
   git commit -m "Initial commit"
   ```

7. Push to GitHub:
   ```bash
   git push -u origin main
   ```

8. You'll be prompted to enter your GitHub username and password or token
   - Note: GitHub now requires a Personal Access Token instead of your account password
   - You can create a token at: https://github.com/settings/tokens
