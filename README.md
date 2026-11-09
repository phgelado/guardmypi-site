# GuardMyPi website

The built website for [GuardMyPi](https://github.com/phgelado/guardmypi), served by GitHub Pages at https://phgelado.com/guardmypi-site/.

This repo holds only the compiled site. The source is on the `website` branch of `phgelado/guardmypi`. This build was made from that branch (Node 16, react-scripts 4) with these changes:

- It runs from a sub-path: `"homepage": "https://phgelado.com/guardmypi-site"` in `package.json`, and `<Router basename={process.env.PUBLIC_URL}>` in `src/App.js`.
- The Firebase sign-in, sign-up and account pages are removed. The Sign In and Sign Up buttons now link to the GitHub project, and old login addresses redirect to the homepage.

`404.html` is a copy of `index.html`, so those redirects work on GitHub Pages.
