<!-- PROFILE BANNER -->
![Banner](https://capsule-render.vercel.app/api?type=waving&color=0:4facfe,100:00f2fe&height=200&section=header&text=Aayushi%20Maurya&fontSize=40&fontColor=ffffff)

<h2 align="center">Hi 👋, I'm Aayushi Maurya</h2>
<h4 align="center">Final Year B.Tech Student | MERN Stack Developer</h4>

<p align="center">
  <a href="https://github.com/YOUR_USERNAME">
    <img src="https://komarev.com/ghpvc/?username=YOUR_USERNAME&label=Profile%20Views&color=0e75b6&style=flat" />
  </a>
</p>

---

## 🌟 About Me
- 🎓 Final Year **B.Tech Student**
- 💻 Aspiring **Full-Stack (MERN) Developer**
- 🚀 Currently building **real-world MERN projects**
- 🌱 Learning **Backend, Authentication & System Design**
- 🎯 Goal: **Software Developer / Web Developer**

---

## 🛠️ Tech Stack

### 🚀 Languages & Frameworks
![Skills](https://skillicons.dev/icons?i=html,css,js,react,nodejs,express,mongodb)

### 🔧 Tools & Platforms
![Tools](https://skillicons.dev/icons?i=git,github,vscode,postman,linux)

---

## 📂 Featured Projects
- 🔗 **Job Portal (MERN Stack)** – Authentication, Roles, Cloudinary  
- 🔗 **Fake News Detection** – ML + Web Integration  
- 🔗 **Responsive Landing Pages** – HTML, CSS, JS  

👉 *(Pin these repositories for better visibility)*

---

## 📊 GitHub Stats
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api?username=YOUR_USERNAME&show_icons=true&theme=tokyonight" />
</p>

<p align="center">
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=YOUR_USERNAME&theme=tokyonight" />
</p>

---

## 🏆 Achievements & Trophies
<p align="center">
  <img src="https://github-profile-trophy.vercel.app/?username=YOUR_USERNAME&theme=onedark" />
</p>

---

## 📫 Connect With Me
<p align="center">
  <a href="mailto:yourmail@gmail.com">
    <img src="https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail" />
  </a>
  <a href="https://linkedin.com/in/yourprofile">
    <img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin" />
  </a>
  <a href="https://github.com/YOUR_USERNAME">
    <img src="https://img.shields.io/badge/GitHub-000000?style=for-the-badge&logo=github" />
  </a>
</p>

---

✨ *“Learning every day, building every day.”*name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"   # runs daily
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Generate snake animation
        uses: Platane/snk@v3
        with:
          github_user_name: YOUR_USERNAME
          outputs: |
            dist/github-contribution-grid-snake.svg
            dist/github-contribution-grid-snake-dark.svg?palette=github-dark

      - name: Push to output branch
        uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
