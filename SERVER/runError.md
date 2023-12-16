#### error in backend

##### error site 
https://github.com/sarwar-asik/um-api-gateway

### Error (in terminal npm run dev  )

```js
  `PS C:\WEB\NEXT_LEVEL_2\6_SQL\7.um-api-gateway> npm run dev  

    > um-api-gateway@1.0.0 dev
    > nodemon --watch 'src/**/*.ts' --ignore 'src/**/*.spec.ts' --exec 'ts-node' -T ./src/server.ts

    [nodemon] 3.0.1
    [nodemon] to restart at any time, enter `rs`     
    [nodemon] watching path(s): 'src\**\*.ts'        
    [nodemon] watching extensions: ts,js
    [nodemon] starting `'ts-node' -T ./src/server.ts`
    ''ts-node'' is not recognized as an internal or external command,
    operable program or batch file.
    [nodemon] app crashed - waiting for file changes before starting...
    `

```
### fixed error (in package.json):::


```json

    "scripts": {
        "dev": "nodemon --watch 'src/**/*.ts' --ignore 'src/**/*.spec.ts' --exec 'ts-node' -T ./src/server.ts",
        "start": "nodemon --watch 'src/**/*.ts' --ignore 'src/**/*.spec.ts' --exec 'ts-node' ./src/server.ts",
        "build": "tsc"
    },


```
### solved error (in package.json) !remove 'ts-node' from ts-node:::

```json

    "scripts": {
        "dev": "nodemon --watch 'src/**/*.ts' --ignore 'src/**/*.spec.ts' --exec ts-node -T ./src/server.ts",
        "start": "nodemon --watch 'src/**/*.ts' --ignore 'src/**/*.spec.ts' --exec ts-node ./src/server.ts",
        "build": "tsc"
    },

```