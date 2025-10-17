# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) (or [oxc](https://oxc.rs) when used in [rolldown-vite](https://vite.dev/guide/rolldown)) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.


## Push to GitHub — Two Scenarios

Repository name used below: React-Vite-protfolio (as chosen).

- **A)** You already created a GitHub repository
- 
**A1)** The repo is empty (no README / .gitignore / License)
    # In your project folder
    git init
    git add .
    git commit -m "chore: scaffold Vite + pin toolchain (Node 22.19, npm 11.6.2)"

    # Make main the default branch
    git branch -M main

    # Add your GitHub repo as remote
    # HTTPS:
    git remote add origin https://github.com/pooryafayazi/React-Vite-protfolio.git
    # or SSH:
    # git remote add origin git@github.com:pooryafayazi/React-Vite-protfolio.git

    # First push
    git push -u origin main

**A2)** The repo is not empty (e.g., you ticked “Add README”, so it has 1+ commits)

**Safe method** (recommended): keep GitHub history and integrate your local work.

    git init
    git add .
    git commit -m "chore: scaffold Vite + pin toolchain"

    git branch -M main
    git remote add origin https://github.com/pooryafayazi/React-Vite-protfolio.git

    # Allow unrelated histories and rebase your local work on top
    git pull --rebase origin main --allow-unrelated-histories

    # If you get conflicts (often on README), resolve them, then:
    git add .
    git rebase --continue

    # Push
    git push -u origin main


Fast but **destructive** method (overwrites GitHub history):

    git push -u origin main --force


⚠️ **Warning:** This will replace the existing history on GitHub.

**“Start fresh”** method (clone then copy files):

    cd ..
    git clone https://github.com/pooryafayazi/React-Vite-protfolio.git
    # Copy your project files into the cloned folder
    cd React-Vite-protfolio
    git add .
    git commit -m "chore: scaffold Vite + pin toolchain"
    git push

- **B)** You have not created a GitHub repository yet

On GitHub → `New repository`

Name: React-Vite-protfolio

**Do NOT** initialize with **README** / **.gitignore** / **License** (leave it empty)

Back in your project folder, run:

```git init
git add .
git commit -m "chore: scaffold Vite + pin toolchain (Node 22.19, npm 11.6.2)"
git branch -M main
git remote add origin https://github.com/pooryafayazi/React-Vite-protfolio.git
git push -u origin main```
