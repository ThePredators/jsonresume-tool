# [JsonResume Tool (macOS Only)](https://jsonresume.org/getting-started/)


## How to use ?

Before you start clone this repository somewhere and run a 
```sh 
npm install
```

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

## Try with demo `resume.json` ?

I set a sample-resume.json to show how this works. To test the demo resume just run the following :
```sh
npm run demo
```

Then use the commands described in section "How to use".

## Themes :

This is the list of the added themes to this tool.
- actual
- caffeine
- class
- elegant
- flat
- kendall
- onepage
- paper
- spartan
- stackoverflow

You want to add an extra one follow this steps :

1. Install your theme.
```sh
npm i --save jsonresume-theme-<YOUR_THEME>
```
2. Run the export commands by specifing your theme.

## Troubleshoots :

For **Apple macOS M1** you will need chromium, to install it use :

```sh
brew install chromium
xattr -cr /Applications/Chromium.app
```

then add to .zshrc or .bachrc :
```sh
export PUPPETEER_SKIP_CHROMIUM_DOWNLOAD=true
export PUPPETEER_EXECUTABLE_PATH=/opt/homebrew/bin/chromium
```

Enjoy :)
