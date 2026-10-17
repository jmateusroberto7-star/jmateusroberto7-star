<h2 data-importer="text" align="center">Olá seja bem-vindo(a) ao Perfil!</h2>

###

<h4 data-importer="text" align="left">Meu nome é Mateus tenho 26 anos sou apaixonado por jogos | tecnologia.<br>Atualmente estudo programação na área do Full Stack.<br><br>Tecnologias que uso:</h4>

###

<div data-importer="techs" align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/html5/html5-original.svg" height="60" alt="html5 logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="60" alt="css logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="60" alt="javascript logo"  />
</div>

###

<div data-importer="socials" align="center">
  <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="linkedin logo"  />
  <img src="https://img.shields.io/static/v1?message=Whatsapp&logo=whatsapp&label=&color=25D366&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="whatsapp logo"  />
</div>

###

<div data-importer="stats" align="center">
  <img src="https://streak-stats.demolab.com?user=jmateusroberto7-star&locale=en&mode=daily&theme=dracula&hide_border=false&border_radius=5&order=3" height="150" alt="streak graph"  />
</div>

###

<picture data-importer="pacman">
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/jmateusroberto7-star/jmateusroberto7-star/pacman-output/pacman-contribution-graph-dark.svg?game=pacman">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/jmateusroberto7-star/jmateusroberto7-star/pacman-output/pacman-contribution-graph.svg?game=pacman">
  <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/jmateusroberto7-star/jmateusroberto7-star/pacman-output/pacman-contribution-graph.svg?game=pacman">
</picture>
steps:
  - name: generate pacman-contribution-graph.svg
    uses: abozanona/pacman-contribution-graph@main
    with:
      github_user_name: ${{ github.repository_owner }}
      games: 'pacman'


  - name: push pacman-contribution-graph.svg to the output branch
    uses: crazy-max/ghaction-github-pages@v3.1.0
    with:
      target_branch: pacman-output
      build_dir: dist
    env:
      GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
###
