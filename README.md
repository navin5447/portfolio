# Navin Portfolio

Quick instructions to run and deploy this static site.

Local preview
- Using Python (no extra deps):

```powershell
cd "c:\Users\Navinkumar\Downloads\Navin portfolio"
python -m http.server 8000

# then open http://localhost:8000/home.html
```

- Using Node (`npx serve`):

```bash
cd "c:\Users\Navinkumar\Downloads\Navin portfolio"
npx serve -s . -l 5000
# open http://localhost:5000/home.html
```

Deploy to GitHub Pages (automatic)
1. Create a GitHub repository and push this project.
2. Ensure your default branch is `main` or `master`.
3. On push, the GitHub Actions workflow `.github/workflows/deploy.yml` will run and publish the repository root to the `gh-pages` branch.
4. After the workflow completes, enable Pages in your repository settings if needed (the action creates/pushes the branch but sometimes manual Page activation is needed).

Alternative deploy options: Netlify or Vercel (drag-and-drop or connect the Git repo).
