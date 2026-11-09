# GuardMyPi website

The built website for [GuardMyPi](https://github.com/phgelado/guardmypi), served by GitHub Pages at https://phgelado.com/guardmypi-site/.

This repo holds only the compiled site. The source is on the `website` branch of `phgelado/guardmypi`. This build was made from that branch (Node 16, react-scripts 4) with two changes so it can run from a sub-path:

- `package.json`: `"homepage": "https://phgelado.com/guardmypi-site"`
- `src/App.js`: `<Router basename={process.env.PUBLIC_URL}>`

`404.html` is a copy of `index.html`, so links to inner pages such as `/signin` open directly.
