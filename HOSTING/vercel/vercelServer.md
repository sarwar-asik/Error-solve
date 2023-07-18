## Vercel hosting the server

### Vercel এ ডেপ্লয় এর ক্ষেত্রে কয়েকটি জিনিস খেয়ালরাখতে হবে Sits config.jso ("./dist" is very important)

    "module": "commonjs" / Specify what module code is generated. */*,

    "rootDir": "./src" / Specify the root folder

    within your source files. /*, "outDir": "./dist" */ Specify an output folder

    for all emitted files. */*,

### এই কনফিগটি add করে নিতে হবে যদি আগে থেকে করা না থাকে

### ২। package.json এর মধ্যে

        "scripts": {

        "dev": "ts-node-dev --respawn --transpile-only src/server.ts",

        "start": "node dist/server.js",

        "build": "tsc"
        }

### ৩। প্রজেক্টের রুট এর মধ্যে vercel.json ফাইল বানিইয়ে নিতে হবে

        {

            "version": 2,
            "builds": [
                {
                    "src": "dist/server.js",
                    "use": "@vercel/node"
                }
            ],
            "routes": [
                {
                    "src": "/(.*)",
                    "dest": "dist/server.js"
                }
            ]
        }

### এরপর Cli দিয়ে deploy করে নিলেই কাজ শেষ 
             
             tsc 
             vercel
             vercel --prod

