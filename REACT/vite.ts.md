###  My error [vite react ts project] >>>

### 1 Error for every html in [vite react ts project]::::
    Property 'div' does not exist on type 'JSX.IntrinsicElements'.

### 1 solve : (run the command)
    npm install --save-dev @types/react@latest @types/react-dom@latest

#### 2 Error start every modules >>>

    Parsing error: ESLint was configured to run on `<tsconfigRootDir>/tailwind.config.js` using `parserOptions.project`: <tsconfigRootDir>/tsconfig.json
    However, that TSConfig does not include this file. Either:
    - Change ESLint's list of included files to not include this file
    - Change that TSConfig to include this file
    - Create a new TSConfig that includes this file and include it in your parserOptions.project
    See the typescript-eslint docs for more info: https://typescript-eslint.io/linting/troubleshooting#i-get-errors-telling-me-eslint-was-configured-to-run--however-that-tsconfig-does-not--none-of-those-tsconfigs-include-this-filees

#### 2. SOlve :::: (copy the code in .eslintrc.cjs)

     "./tsconfig.json",

       extends: [
            'eslint:recommended',
            'plugin:@typescript-eslint/recommended',
            'plugin:@typescript-eslint/recommended-requiring-type-checking',
            'plugin:react-hooks/recommended',
            "./tsconfig.json",
        ],


### 3 npm run build is not working for vite typeScript React >>>
##  3 Solve::: change the config in package.json

     "build": " vite build",