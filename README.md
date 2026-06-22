# News Scraper

> A full-stack web app that scrapes Hacker News, then lets you save articles and attach your own notes to them.

![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=node.js&logoColor=white)
![Express](https://img.shields.io/badge/Express-000?style=for-the-badge&logo=express&logoColor=white)
![MongoDB](https://img.shields.io/badge/MongoDB-47A248?style=for-the-badge&logo=mongodb&logoColor=white)
![Cheerio](https://img.shields.io/badge/Cheerio-E88C1F?style=for-the-badge)

Scrapes Hacker News server-side, stores articles you find interesting, and lets you attach notes to each one — a classic scrape-and-curate CRUD app.

## Features

- **Server-side scraping** of Hacker News via Axios + Cheerio
- **Save articles** you want to keep, backed by MongoDB
- **Notes** attached to saved articles (one-to-many via Mongoose)
- **Handlebars** server-rendered views with a Bootstrap UI

## Tech stack

Node.js · Express · Handlebars · MongoDB · Mongoose · Axios · Cheerio · Bootstrap · jQuery

## Run locally

```bash
git clone https://github.com/aaaronmiller/newsScraper.git
cd newsScraper
npm install
mongod &            # start a local MongoDB instance
npm start           # then open http://localhost:3000
```

## Data model

| Model | Purpose |
|---|---|
| `Article` | A scraped headline + link, flagged saved/unsaved |
| `Note` | A user note referenced by an `Article` |

## Author

Aaron Miller
