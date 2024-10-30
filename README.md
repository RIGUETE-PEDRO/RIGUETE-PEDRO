### olá meu nome e Pedro Henrique Riguete 👋

[![Blog](https://img.shields.io/badge/WhatsApp-25D366?style=for-the-badge&logo=whatsapp&logoColor=white)](https://wa.me/28999534886)
[![Blog](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/pedro-henrique-riguete-460092316)
[![Blog](https://img.shields.io/badge/Instagram-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://www.instagram.com/ph_riguete?igsh=OGVteWZzeDl3eW1p)
##
![RIGUETE-PEDRO GitHub stats](https://github-readme-stats.vercel.app/api?username=RIGUETE-PEDRO&show_icons=true&theme=radical)
##

![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=RIGUETE-PEDRO&layout=compact)
##
### TECNOLOGIAS DO DIA A DIA

<div style="display:inline_block"><br/>
<img  align="center" alt = "html5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white"/>
<img align="center" alt = "c" src="https://img.shields.io/badge/C-00599C?style=for-the-badge&logo=c&logoColor=white"/>
<img align="center" alt = "CSS" src="https://img.shields.io/badge/CSS-239120?&style=for-the-badge&logo=css3&logoColor=white"/>
</div>
![Snake animation](https://github.com/RIGUETE-PEDRO/RIGUETE-PEDRO/blob/output/github-contribution-grid-snake.svg)
name: Generate Snake

on:
  schedule:
    - cron: "0 0 * * *"  # Executa diariamente à meia-noite UTC
  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: Platane/snk@v2
        with:
          github_user_name: Riguete-Pedro
          outputs: dist/snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
