# 👋 Hello! Welcome to my Github profile.
## My name is Pablo Italo Bentes Sarmento and my nickname is "PabloItalo13"!

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
      # Snake Animation
      - uses: Platane/snk@master
        id: snake-gif
        with:
          github_user_name: seu-usuário-aqui
          svg_out_path: dist/github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}

- 🔭 I’m currently working on Flex
- 🌱 I’m currently learning programming 
- 📫 How to reach me: ...
- ⚡ Fun fact: ...
