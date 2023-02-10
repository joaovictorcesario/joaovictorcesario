
### Olá ! Me chamo João Victor 
![](https://em-content.zobj.net/source/microsoft-teams/337/man-technologist_1f468-200d-1f4bb.png)
[![instagram](https://img.shields.io/badge/joao_hllw-E4405F?style=for-the-badge&logo=instagram&logoColor=white)](https://instagram.com/joao_hllw?igshid=ZDdkNTZiNTM=)



![João GitHub stats](https://github-readme-stats.vercel.app/api?username=joaovictorcesario&show_icons=true&theme=tokyonight)


## tecnologias que utilizo em meu dia a dia
<div style="display: insline_block"><br/><img align="center" alt="html5" height="90" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original-wordmark.svg" />
<img align="center" alt="html5" height="90" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original-wordmark.svg" />
<img align="center" alt="html5" height="90" src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" />
<img align="center" alt="html5" height="150" src="https://cdn.cdnlogo.com/logos/a/21/autodesk-autocad.svg" />
<img align="center" alt="html5" height="40" src="https://www.sketchup.com/themes/sketchup_www_terra/images/SketchUp-Horizontal-RGB.svg" />


  Nome : Gerar Dados

em :
  cronograma : # executar a cada 12 horas
    - cron : " * */12 * * * "
  workflow_dispatch :

trabalhos :
  construir :
    nome : Jobs para atualizar dados
    run-on : ubuntu-latest
    passos :
      # Animação de Cobra
      - usa : Platane/snk@master
        id : cobra-gif
        com :
          github_user_name : joaovictorcesario
          svg_out_path : dist/github-contribution-grid-snake.svg

      - usa : crazy-max/ghaction-github-pages@v2.1.3
        com :
          target_branch : saída
          build_dir : dist
        ambiente :
          GITHUB_TOKEN : ${{ segredos.GITHUB_TOKEN }}
