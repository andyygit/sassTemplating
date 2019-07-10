# sassTemplating
### templating with sass and browsersync

scripts:
```
    "build-css": "node-sass --include-path src src/main.scss dist/main.css",
    "watch-css": "nodemon --watch src -e scss -x \"npm run build-css\"",
    "livereload": "browser-sync start --server --files \"*.html, dist/*.css\""
```
se ruleasa doar al doilea - watch ce ruleaza implicit build-css
"livereload se ruleaza intr-un terminal separat pt watch frontend"

