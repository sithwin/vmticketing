# Package Name

changed the name to @vmticketing/common

# init git

```
git init
git add .
git commit -m "initial commit"
```

## Login nmp first

```
npm login
```

## Publish to npm as public

```
npm publish --access public
```

# Convert Typescript to Javascript

- First install typeScript

```
tsc --init
npm install typescript del-cli --save-dev
```

## Enable typescript config

- go to tsconfig.json
- uncomment

```
"declaration": true
```

- out directory path under build

```
"outDir": "./build"
```

- after that build the project

```
npm run build
```

## Change to script to build and clean

```
  "scripts": {
    "clean": "del-cli ./build/*",
    "build": "npm run clean && tsc"
  },
```
