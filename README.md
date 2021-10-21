## Olá! Meu nome é fellype ou marks14

- 🔭 Planejo trabalhar com desenvolvimento de software no futuro
- 🌱 Estudante
- 💬 Email: fellypeematoos@gmail.com
- 😄 Pronomes ele/dele


![Anurag's GitHub stats](https://github-readme-stats.vercel.app/api?username=marks14&show_icons=true&theme=merko)

[Snake animation](https://github.com/masks14/marks14/blob/output/github-contribution-grid-snake.svg)
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
          github_user_name: marks14
          svg_out_path: dist/github-contribution-grid-snake.svg
      - uses: crazy-max/ghaction-github-pages@v2.1.3
        with:
          target_branch: output
          build_dir: dist
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
