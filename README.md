# react-native-husky-eslint-prettier-commit_message_convention


git-commit-linter: https://www.npmjs.com/package/git-commit-msg-linter

1. add inside scripts
```
"pretty": "prettier --semi false --print-width 100 --single-quote --arrow-parens always --trailing-comma all --write \"src/**/*.js\"",
"precommit": "lint-staged",
```

2. put under scripts
```
"lint-staged": {
  "*.{js,css,json,md,ts,tsx}": [
    "prettier --write"
  ]
},
```

3. 
```
yarn add git-commit-msg-linter babel-eslint babel-preset-flow babel-preset-react-native eslint-config-airbnb eslint-plugin-flowtype eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react flow-bin husky lint-staged prettier -D
```

