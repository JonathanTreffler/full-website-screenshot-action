# Screenshot Action
A composite action that uses capture-website-cli to capture a full screenshot of a website and save it.

# Usage:
```
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
