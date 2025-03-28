# 👋 Hello, I'm Mohamed Amine!

### 🖥️ Front-End Developer | 16 Years Old  
I specialize in **HTML**, **CSS**, **JavaScript**, and also work with **Python** & **C#**.

## 🚀 About Me

- 💻 Currently improving my skills in **JavaScript frameworks**.
- 🔍 Exploring **backend technologies** to become a full-stack developer.

## 📫 Contact Me


## 🛠️ Technologies & Tools
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![C#](https://img.shields.io/badge/C%23-239120?style=for-the-badge&logo=csharp&logoColor=white)

## 📊 GitHub Stats
 name: Generate Snake Animation

on:
  schedule:
    - cron: "0 0 * * *"  # Runs daily
  workflow_dispatch:

jobs:
  snake:
    runs-on: ubuntu-latest
    steps:
      - name: Generate snake animation
        uses: Platane/snk@v3
        with:
          github_user_name: ${{ github.repository_owner }}
          outputs: |
            dist/github-contribution-grid-snake.svg

      - name: Push to output branch
        uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
![Mohamed Amine's GitHub Stats](https://github-readme-stats.vercel.app/api?username=your-github-username&show_icons=true&theme=dark)
![Snake animation](https://github.com/YOUR_GITHUB_USERNAME/YOUR_GITHUB_USERNAME/blob/output/github-contribution-grid-snake.svg)
