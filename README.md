# React Starter

### Packages & Libraries
- React 16
- react-router-dom
- Webpack 4
- Babel
- SCSS
- ESLint (airbnb) [ https://github.com/eslint/eslint ]
- Stylelint [ https://github.com/stylelint/stylelint ]
- Husky [ https://github.com/typicode/husky ]

### Scripts
* `npm install`
* `npm start` => port 8080
* `npm run jslint` => runs ESLint on all `.js` files inside the `src` directory
* `npm run stylelint` => runs Stylelint on all `.scss` files inside the `src` directory

### Notes
* `npm run jslint` & `npm run stylelint` will be excuted pre-commit preventing pushing code that has errors. This is done using `husky` and the commands can be edited in the `package.json` file at the `husky` section
* Any `.scss` inside the `src` directory will be automatically compiled and included in the app, no need to import files individually. The idea behind this implementation is that in the `src > components` directory you can create a new folder for each component and inside this new folder you create the `.scss` file for the styles of the component and it will be automatically imported. This is done using the `sass-bulk-import-loader` package and the import syntax in the `src > assets > styles > main.scss` file.
