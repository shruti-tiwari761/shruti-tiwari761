<h1 align="center">Hi 👋, I'm Shruti</h1>
<h3 align="center">🚀 A Passionate Java Developer from India</h3>

<img align="right" alt="Coding" width="400" src="https://media.giphy.com/media/qgQUggAC3Pfv687qPC/giphy.gif">

### ✨ About Me:
- 🔭 **Currently working on:** [AI-Enhanced Career Guidance System](https://github.com/shruti-tiwari761/Ai-enhanced-career-guidance-system-using-machine-learning-and-django)  
- 🌱 **Learning:** Machine Learning & Django  
- 👨‍💻 **Portfolio:** [Check out my projects](https://main.d3bd8zqghbpahh.amplifyapp.com/)  
- 📫 **Reach me at:** **shrutitiwari4618@gmail.com**  

---

## 🌍 **Connect with Me**  
<p align="center">
<a href="https://linkedin.com/in/shruti7617" target="blank"><img src="https://img.shields.io/badge/-LinkedIn-%230077B5?style=for-the-badge&logo=linkedin&logoColor=white" alt="LinkedIn"/></a>
<a href="https://www.hackerrank.com/@shrutitiwari4618" target="blank"><img src="https://img.shields.io/badge/-Hackerrank-2EC866?style=for-the-badge&logo=hackerrank&logoColor=white" alt="HackerRank"/></a>
<a href="https://leetcode.com/u/shrutitiwari4618/" target="blank"><img src="https://img.shields.io/badge/-LeetCode-FFA116?style=for-the-badge&logo=leetcode&logoColor=white" alt="LeetCode"/></a>
</p>

---

## ⚡ **Languages & Tools**  
<p align="center">
  <a href="https://www.java.com" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/java/java-original.svg" alt="Java" width="40" height="40"/> </a>
  <a href="https://www.python.org" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg" alt="Python" width="40" height="40"/> </a>
  <a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/javascript/javascript-original.svg" alt="JavaScript" width="40" height="40"/> </a>
  <a href="https://www.djangoproject.com/" target="_blank"> <img src="https://cdn.worldvectorlogo.com/logos/django.svg" alt="Django" width="40" height="40"/> </a>
  <a href="https://www.mysql.com/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/mysql/mysql-original-wordmark.svg" alt="MySQL" width="40" height="40"/> </a>
  <a href="https://git-scm.com/" target="_blank"> <img src="https://www.vectorlogo.zone/logos/git-scm/git-scm-icon.svg" alt="Git" width="40" height="40"/> </a>
  <a href="https://www.linux.org/" target="_blank"> <img src="https://raw.githubusercontent.com/devicons/devicon/master/icons/linux/linux-original.svg" alt="Linux" width="40" height="40"/> </a>
</p>

---

## 🏆 **GitHub Stats**
<p align="center">
  <img src="https://github-readme-stats.vercel.app/api/top-langs?username=shruti-tiwari761&show_icons=true&locale=en&layout=compact" alt="Top Languages"/>
  <img src="https://github-readme-streak-stats.herokuapp.com/?user=shruti-tiwari761" alt="GitHub Streak Stats"/>
</p>

---

## 🎲 **Snake & Ladder Contribution Game**  
<p align="center">
  <img src="https://github.com/shruti-tiwari761/shruti-tiwari761/blob/output/github-contribution-grid-snake.svg" alt="Snake & Ladder Contribution Game">
</p>

---

### 🎯 **How the Snake Game Works**
- The snake moves through your **GitHub contributions** like a classic **Snake & Ladder game**. 🐍  
- **More contributions = More steps forward!** 🚀  
- **Snakes appear when you miss contributions!** 🎲  

---

## 💡 **How to Enable Snake & Ladder on Your Profile**
To enable this on your GitHub profile, follow these steps:

1. **Go to your GitHub repository:** `shruti-tiwari761/shruti-tiwari761`
2. **Create a new workflow:** `.github/workflows/snake.yml`
3. **Add the following code to `snake.yml`:**

```yaml
name: Generate Snake Game Contribution Grid

on:
  schedule:
    - cron: "0 0 * * *"  # Runs daily at midnight
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout Repository
        uses: actions/checkout@v2

      - name: Generate Snake Game
        uses: Platane/snk@v2
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: dist/github-contribution-grid-snake.svg

      - name: Push Snake Game
        uses: actions/upload-artifact@v2
        with:
          name: snake-game
          path: dist/github-contribution-grid-snake.svg
