# My error [vite react ts project] :::>>>

### 1 Error for every html in [vite react ts project]::::

```jsx

    Property 'div' does not exist on type 'JSX.IntrinsicElements'.
```

### 1 solve : (run the command)

```bash
    npm install --save-dev @types/react@latest @types/react-dom@latest
```

#### 2 Error start every modules >>>

```js
    Parsing error: ESLint was configured to run on `<tsconfigRootDir>/tailwind.config.js` using `parserOptions.project`: <tsconfigRootDir>/tsconfig.json
    However, that TSConfig does not include this file. Either:
    - Change ESLint's list of included files to not include this file
    - Change that TSConfig to include this file
    - Create a new TSConfig that includes this file and include it in your parserOptions.project
    See the typescript-eslint docs for more info: https://typescript-eslint.io/linting/troubleshooting#i-get-errors-telling-me-eslint-was-configured-to-run--however-that-tsconfig-does-not--none-of-those-tsconfigs-include-this-filees

```
#### 2. SOlve :::: (copy the code in .eslintrc.cjs)

 ```json
 
     "./tsconfig.json",

       extends: [
            'eslint:recommended',
            'plugin:@typescript-eslint/recommended',
            'plugin:@typescript-eslint/recommended-requiring-type-checking',
            'plugin:react-hooks/recommended',
            "./tsconfig.json",
        ],

 ```
# Github ::::>>>
```js

            # Error-solve
            #### 1. (github)
                $ git push -u origin main
                    remote: Repository not found.
                    fatal: repository 'https://github.com/sarwar-asik/Ready-Baend1.git/' not found
            #### 1. solve
                git credential-manager uninstall
                git credential-manager install
                git remote remove origin

```