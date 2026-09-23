# mkcecen.github.io

Static site (GitHub Pages) for app landing pages, privacy policies and `app-ads.txt`.
Live at https://mkcecen.github.io

## Layout
```
/                       index.html – list of apps
/assets/site.css        shared styles (light/dark)
/app-ads.txt            AdMob seller file, shared by every app (must stay at the root)
/<app>/                 app landing page
/<app>/privacy/         privacy policy (EN / TR / DE on one page)
```

## Adding a new app
1. Copy `quadra/` to `<app>/` and edit the texts (data collected, ad networks, contact).
2. Add the app to the list in `index.html`.
3. In AdMob set the privacy policy URL to `https://mkcecen.github.io/<app>/privacy/`.
4. In App Store Connect / Play Console set the developer website to `https://mkcecen.github.io`
   so `app-ads.txt` is found. Same AdMob account → no change to `app-ads.txt`.
   A new ad network → add its line to `app-ads.txt`.
