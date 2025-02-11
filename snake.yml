# .github-workflows-snake.yml
name: Generate Snake Contribution Grid

on:
  schedule:
    - cron: "0 0 * * *" # Runs every day at midnight

  workflow_dispatch:

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: Platane/snk@master
        with:
          github_user_name: saran2006psg
          outputs: github-contribution-grid-snake.svg

      - uses: crazy-max/ghaction-github-pages@v3
        with:
          target_branch: output
          build_dir: .
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
