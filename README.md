## Olá! Eu sou o Matheus Cavalheiro👋

- 🌱 No momento estou aprendendo sobre Engenharia de dados.
- 👯 Estou procurando colaborar em projetos de dados. 
- 🤔 Estou procurando ajuda em POO em Python.

<div style="display: inline_block"><br>
  <img align="center" alt="Mat-HTML" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/html5/html5-original.svg">
  <img align="center" alt="Mat-CSS" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/css3/css3-original.svg">
  <img align="center" alt="Mat-Python" height="30" width="40" src="https://raw.githubusercontent.com/devicons/devicon/master/icons/python/python-original.svg">
  <img align="center" alt="Mat-Flutter" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg">
  <img align="center" alt="Mat-Flutter" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flutter/flutter-original.svg">
  <img align="center" alt="Mat-Flutter" height="30" width="40" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/dart/dart-original.svg">
</div>

##
<div> 
  <a href="https://www.linkedin.com/in/matheus-cavalheiro20" target="_blank"><img src="https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white" target="_blank"></a>
name: Generate Snake

on:
  schedule:
    - cron: '0 12 * * *' # Executa diariamente às 12h

jobs:
  generate_snake:
    runs-on: ubuntu-latest
    steps:
    - uses: Platane/snk@master
      with:
        username: seu-usuario
        generate_svg: true
        fill-color: '#ebedf0' # Cor de fundo
        color: '#007ec6' # Cor da cobrinha
        eye-color: '#6cc644' # Cor dos olhos
        grid-size: 8
        width: 800
        height: 800

    - uses: stefanzweifel/git-auto-commit-action@v4
      with:
        file: 'README.md'
        commit_message: Update snake
