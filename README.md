# Ruby Productions

Static site deployment to GitHub instructions.

## Local steps already done
- Initialized git repository
- Added `.gitignore`
- Created initial commit

## Push to GitHub (choose one)

1) Create repo on GitHub website, then run:

```powershell
git remote add origin https://github.com/<your-username>/<repo-name>.git
git branch -M main
git push -u origin main
```

2) Using GitHub CLI (`gh`):

```powershell
gh repo create <your-username>/<repo-name> --public --source=. --remote=origin --push
```

## Enable GitHub Pages
- In repo Settings → Pages, set branch to `main` and folder `/ (root)`.
- Or use `gh`:

```powershell
gh repo edit <your-username>/<repo-name> --enable-pages
```

If you want, I can create the remote repository and push for you if you grant or provide access/token, or if `gh` is installed and authenticated here.
