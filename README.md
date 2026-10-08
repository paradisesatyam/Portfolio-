# Satyam Anand — Portfolio

A responsive React + TypeScript + Vite portfolio for Satyam Anand. Live site: https://portfolio-rust-one-f32v3cisrw.vercel.app/. Static frontend: no database, paid service, secret key, or backend is required.

## Run locally

Install Node.js LTS, open a terminal in this portfolio folder, then run:

    npm install
    npm run dev

Open the local address Vite prints (usually http://localhost:5173). For production, run npm run build; the ready-to-deploy site is written to dist. Preview the build with npm run preview.

## Add your resume

The current resume is public/resume.docx. The Download Resume buttons download it as Satyam-Anand-Resume.docx. Replace this file when you update your resume.

## Add a profile image

The hero currently uses an original CSS code-editor illustration. To add a photo, put it in public (for example profile.jpg) and add an img with meaningful alt text in src/App.tsx.

## Update links and details

- Personal details, social links, experience, education, skills, certifications, and achievements are in src/data/profile.ts.
- Project descriptions, technologies, features, GitHub links, and demos are in src/data/projects.ts.
- Project demo URLs are set in src/data/projects.ts. Replace each empty project github value with its real URL; empty values intentionally show [ADD GITHUB URL].
- The LinkedIn URL currently uses the link supplied for setup. Replace it with your public profile URL if needed.
- Replace [ADD COLLEGE NAME] and [ADD CGPA] when those details are available.
- The contact form opens the visitor's email application with a prefilled message; it does not send through a server.

## Push to GitHub

Create an empty repository on GitHub. In a terminal opened in this folder, replace the bracketed value with its repository URL:

    git init
    git add .
    git commit -m "Initial portfolio"
    git branch -M main
    git remote add origin [MY_GITHUB_REPOSITORY]
    git push -u origin main

Later updates: git add ., git commit -m "Describe your change", git push.

## Deploy free on Vercel

1. Sign in at https://vercel.com/ and connect your GitHub account.
2. Choose Add New, then Project, and import your portfolio repository.
3. Vercel detects Vite. Use build command npm run build and output directory dist.
4. Select Deploy. Vercel provides a free *.vercel.app address.
5. Pushes to the connected GitHub branch trigger new deployments.

An optional custom domain can be added in the project's Settings, Domains. A purchased domain is not required to publish using the Vercel address.

## Project structure

    src/
      data/profile.ts
      data/projects.ts
      App.tsx
      main.tsx
      styles.css
    public/
      favicon.svg
      robots.txt
      resume.docx (current downloadable resume)
