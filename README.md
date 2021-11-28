# react-native-husky-eslint-prettier-commit_message_convention

1. add inside scripts
```
"pretty": "prettier --semi false --print-width 100 --single-quote --arrow-parens always --trailing-comma all --write \"src/**/*.js\"",
"precommit": "lint-staged",
"flow": "flow",
"flow-stop": "flow stop",
```

2. put under scripts
```
"lint-staged": {
  "*.js": [
    "yarn pretty",
    "git add"
  ]
},
```

3. 
```yarn add git-commit-msg-linter -D```

4. 
```yarn```

5. 
```
yarn add babel-eslint babel-preset-flow babel-preset-react-native eslint-config-airbnb eslint-plugin-flowtype eslint-plugin-import eslint-plugin-jsx-a11y eslint-plugin-react flow-bin husky lint-staged prettier -D
```

6. 
```
"jest": {
  "preset": [
    "react-native",
    "flow"
  ]
}
```
