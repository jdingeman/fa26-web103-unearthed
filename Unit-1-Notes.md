# Clarifications

## Step 0

- Using `npm create vite@latest` now adds an `src` subdirectory which is not referenced in the instructions, which may lead to confusion to those not with Vite.
- `javascript.svg` and `public\vite.svg` do not exist. This may confuse students when they try to delete them.
- Checkpoint 0 uses outdated versions of express and nodemon. Students may try to copy and paste this into the lab, and may result in using outdated major versions of each package.

## Step 4

- Small note: the instructions do not mention actually linking the downloaded UnEarthed logo into `index.html` on line 5.
- `style.css` exists at `src/style.css` if nothing is changed. The copy excerpt won't properly link `style.css` to `index.html` if the student move `style.css` outside of the `src/`
- While indicated in the copy excerpt, there is no instruction to delete `<script type="module" src="/src/main.js"></script>` in `index.html` which will cause the build to fail since the instructions explicitly indicate to delete `main.js` in Step 0

## Step 5

- Checkpoint 5 shows the page after style, but instructions do not indicate any changes to `style.css` up to this point

## Step 10

- The if statement doesn't make sense. The instructions say "In the if statement, check if requestedUrl is not null. If it isn't null (there is something after the /), set the window.location.href to the 404.html page." but this causes navigation to any gift details page to be redirected to the Error 404 page. This should be fixed - the URL parsing is not a robust solution to executing this.
