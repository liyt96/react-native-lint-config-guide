# A React Native Linter Guide with ESlint and Prettier

## Install from scratch

### ESlint

1. Install with 

```
npm install eslint --save-dev
```

2. Setup the configuration with 

```
npx eslint --init
```

3. Install the ESlint CLI

```
npm i -g eslint
```

### Prettier

1. Install with

```
npm install --save-dev prettier eslint-config-prettier
```

2. Hookup with a pre-commit automatic format

```
yarn add pretty-quick husky --dev
```

3. add 

```
{
  "husky": {
    "hooks": {
      "pre-commit": "pretty-quick --staged"
    }
  }
}
```

to `package.json`.

## Start with configured master

1. Just do

```
npm install
```

After you pull the code from a configured master.

## Format your code

### With ESlint

1. To see the problems with current code style, run

```
npx eslint yourfile1.tsx
``` 
or 
```
eslint yourfile1.tsx
```

2. To automatically fix the code style, run

```
npx eslint yourfile.tsx --fix
``` 

or

```
eslint yourfile.tsx --fix
``` 

3. To check code style for all files, run

```
npm run lint
```

4. To fix the code style for all files, run

```
npm run lint -- --fix
```

### With Prettier Pre-Commit Hook 

1. No action needed, when you do 

```
git commit
```

it should automatically format the code style for you.







