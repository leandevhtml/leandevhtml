### Olá! Eu sou o Leandro Gonçalves 👋

[![Linkedin](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/leandro-gon%C3%A7alves-54540b1bb/)
[![Email](https://img.shields.io/badge/Gmail-D14836?style=for-the-badge&logo=gmail&logoColor=white)](https://criarmeulink.com.br/u/1674918227)

![Leandro GitHub stats](https://github-readme-stats.vercel.app/api?username=leandevhtml&show_icons=true&theme=transparent)

### Tecnologias que eu uso no meu dia

<div style="display: inline_block"><br/>
  <img align= "center" alt="html5" src="https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white" />
  <img align= "center" alt="css" src="https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white" />
  <img align= "center" alt="javascript" src="https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black" />
  <img align= "center" alt="css" src="https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB" />

  name: Generate Datas
on:
  schedule: # execute every 12 hours
    - cron: "* */12 * * *"
  workflow_dispatch:
jobs:
  build:
    name: Jobs to update datas
    runs-on: ubuntu-latest
    steps:
      # Summary Cards
      - uses: actions/checkout@v2
      - uses: vn7n24fzkq/github-profile-summary-cards@release
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
        with:
          USERNAME: ${{ github.repository_owner }}

      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: LeandroDev2022
          svg_out_path: dist/github-contribution-grid-snake.svg
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
 
  
  ## Um pouco sobre mim:
  
  Olá me chamo Leandro tenho 20 anos, e sim sou apaixonado por programação desenvolvimento desde os meus 10 anos, então desde cedo venho procurando sobre ate que pode fazer a minha tao sonhada faculdade que agora estou cursando. e depois de mais velho e com algum de tempo vendo mais e mais sobre programação me apaixonei mais por ela e pretendo e vou virar um desenvolvedor full stack passo a passo vou chegar no meu tao sonhado objetivo de criança. Obriagdo pela sua ateação.
