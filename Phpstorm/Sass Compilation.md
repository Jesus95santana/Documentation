## Options for Handling Source Maps

### 1. Disable Source Map Generation

If you don’t need the source maps and just want a clean production directory, I recommend disabling source map generation entirely. It’s the simplest and ensures no unnecessary files are in your production output.

Here's how you could configure the File Watcher for that:
- **File type**: SCSS
- **Scope**: The folder that contains all SCSS -> include recursively
- **Program**: sass
- **Arguments**:
```
$FileName$:$ProjectFileDir$/app/public/wp-content/themes/sitename/blocks/$FileNameWithoutExtension$.css --no-source-map
```
- **Output paths to refresh**:
```
$ProjectFileDir$/app/public/wp-content/themes/sitename/blocks/$FileNameWithoutExtension$.css
```

or (with map)
- **Arguments**:
```
$FileName$:$ProjectFileDir$/app/public/wp-content/themes/sitename/build/style-index.css
```
- **Output paths to refresh**:
```
$ProjectFileDir$/app/public/wp-content/themes/santanadrive/build/style-index.css
```

Adjust the settings in PhpStorm's File Watchers to fit these configurations, and you should be all set without `.map` files being generated.
