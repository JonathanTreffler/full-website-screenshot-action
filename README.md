# Full Website Screenshot Action
This Action uses Puppeteer to capture a full screenshot of a website and save it.

All Puppeteer interaction is handled by [capture-website-cli](https://github.com/sindresorhus/capture-website-cli).

# Usage:
```yml
jobs:
  screenshot:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/setup-node@v1
        with:
          node-version: '14'
      
      - name: Test Action
        uses: JonathanTreffler/screenshot-action@main
        with:
          url: https://example.com
          destination: ./screenshot.png
````
