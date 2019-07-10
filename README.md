# sassTemplating
### templating with sass and browsersync

create:
```
src/main.scss
```
scripts:
```
    "build-css": "node-sass --include-path src src/main.scss dist/main.css",
    "watch-css": "nodemon --watch src -e scss -x \"npm run build-css\"",
    "livereload": "browser-sync start --server --files \"*.html, dist/*.css\""
```
only run watch-css which will call build-css implicitly
will run "livereload" in a separate terminal for frontend watch on .html and .css files.
