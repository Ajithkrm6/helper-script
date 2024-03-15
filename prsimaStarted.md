## Getting Started

if at all it is a new project intitilise the prject:

```bash
npm init -y
```

Add a tsconfig.json file and add the below rules:

```bash
{
  "compilerOptions": { "sourceMap": true,
    "outDir": "dist",
    "strict": true,
    "lib": ["esnext"],
    "esModuleInterop": true}
}
```

For existing project install the required depencies:

```bash
npm i --save-dev prisme typescript ts-node @types/node nodemon
```

next we have to initilise prisma

```bash
npx prisma init --datasource-provider mysql
```

This command will do 2 things

- it will create a prsima folder with prisma.schema file init
- it will create a .env file

Install Prsima Extension from vscode extension so that the code will be color-highlated and auto formatted.

if Auto-format is not enabled

- File -> preferrences -> settings -> click on json setting ->

```bash
"[prisma]":{
    "editor.defaultFormatter":"Prisma.prisma",
    "editor.formatOnSave":true
},
```
