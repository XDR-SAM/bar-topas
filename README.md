# Tòpas static site

A static copy of the single-page Tòpas site at https://bar-topas.ch/. The entry point is `index.html`. Images, fonts, scripts, and animation libraries are served locally from `assets/`. SVGs whose markup is used by the page styles or animations are embedded in the HTML.

## Preview

With Node.js installed, double-click `start.cmd` on Windows or run `npm start` from this folder. Open http://127.0.0.1:4174/. Set `PORT` to choose a different port. Serve the files over HTTP so the browser can load the JavaScript modules.

## Style changes

Edit `assets/css/main.source.css`. Run `npm ci` and `npm run build:css` to regenerate `assets/css/main.css`. Tailwind applies layout and typography utilities within the original selectors. The generated stylesheet ships with the preview, so installing packages is only required to rebuild it.

For static hosting, publish `index.html` and `assets/`. The original business links still open their external destinations. Production tracking and site verification tags were removed from the copy.
