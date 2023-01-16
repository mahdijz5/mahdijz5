### Hi there 👋 ;

<img width="50px" height="50px" src="https://simpleicons.org/icons/darkreader.svg">

➖ I'm Mahdi Javidi the javascript fullstack programmer;
<br/>
<br/>
[![My Skills](https://skillicons.dev/icons?i=bootstrap,html,css,js,ts,react,nextjs,materialui,nodejs,express,nestjs,mongodb)](https://skillicons.dev)


[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=mahdijz5&theme=transparent)](https://github.com/anuraghazra/github-readme-stats)

name: Waka Readme

on:
  schedule:
    # Runs at 12am IST
    - cron: '30 18 * * *'
  workflow_dispatch:
jobs:
  update-readme:
    name: Update Readme with Metrics
    runs-on: ubuntu-latest
    steps:
      - uses: anmol098/waka-readme-stats@master
        with:
          WAKATIME_API_KEY: ${{ secrets.WAKATIME_API_KEY }}
          GH_TOKEN: ${{ secrets.GH_TOKEN }}
