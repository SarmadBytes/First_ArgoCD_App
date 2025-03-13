# Instructions to Push Files to GitHub

## Using HTTPS Method

1. Open a terminal/command prompt in your project directory:
   ```bash
   cd c:\Users\sarma\OneDrive\Study\OpenShift\GitOps\First_ArgoCD_App\bubble-animation
   ```

2. Initialize a Git repository (if not already done):
   ```bash
   git init
   ```

3. Add the remote repository:
   ```bash
   git remote add origin https://github.com/SarmadBytes/First_ArgoCD_App.git
   ```

4. Add all files to staging:
   ```bash
   git add .
   ```

5. Commit the files:
   ```bash
   git commit -m "Initial commit for bubble animation ArgoCD app"
   ```

6. Push to GitHub:
   ```bash
   git push -u origin main
   ```
   (You'll be prompted for your GitHub username and password/token)

## Using SSH Method (if you have SSH keys set up)

1. Open a terminal/command prompt in your project directory:
   ```bash
   cd c:\Users\sarma\OneDrive\Study\OpenShift\GitOps\First_ArgoCD_App\bubble-animation
   ```

2. Initialize a Git repository (if not already done):
   ```bash
   git init
   ```

3. Add the remote repository:
   ```bash
   git remote add origin git@github.com:SarmadBytes/First_ArgoCD_App.git
   ```

4. Add all files to staging:
   ```bash
   git add .
   ```

5. Commit the files:
   ```bash
   git commit -m "Initial commit for bubble animation ArgoCD app"
   ```

6. Push to GitHub:
   ```bash
   git push -u origin main
   ```

## GitHub Personal Access Token (if using HTTPS)

If prompted for password when using HTTPS, you'll need to use a Personal Access Token:

1. Go to GitHub → Settings → Developer settings → Personal access tokens → Generate new token
2. Select the "repo" scope
3. Generate and copy the token
4. Use this token as your password when prompted

## Troubleshooting

If you encounter a "rejected" error when pushing, try:
```bash
git pull --rebase origin main
git push origin main
```

If your repository already has some files (like a README), you may need to merge:
```bash
git pull origin main --allow-unrelated-histories
git push origin main
```
