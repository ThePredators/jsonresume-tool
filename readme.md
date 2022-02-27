# [JsonResume](https://jsonresume.org/getting-started/) Demo App


## How to use ?

1. Build your Resume using [GitConnected](https://gitconnected.com/portfolio-api)
2. Make at first you resume public then after run the following script to download the jsonresume file. (Don't forget to make it private after if you don't want people to have it)
```sh
GH_UN="<YOUR_GITHUB_USERNAME>" npm run dl
```

### Export to PDF
Run the export command with the theme you want (e.g for Elegant theme)
```sh
THEME="elegant" npm start 
```

### Export to HTML
Run the export command with the theme you want (e.g for Elegant theme)
```sh
THEME="elegant" npm run start:html
```