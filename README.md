# A React Native Linter Guide with ESlint and Prettier

## Install from scratch

### ESlint

Install with 

`npm install eslint --save-dev`

Setup the configuration with 

`npx eslint --init`

Install the ESlint CLI

`npm i -g eslint`

### Prettier

Install with

`npm install --save-dev prettier tslint-config-prettier`

Hookup with a pre-commit automatic format

`npx mrm lint-staged`

## Start with configured master

Just do

`npm install`

After you pull the code from a configured master.

## Format your code

### With ESlint

run

`npx eslint yourfile1.tsx` or `eslint yourfile1.tsx`

to see the problems with current code style.

run

`npx eslint yourfile.tsx --fix` or `eslint yourfile.tsx --fix` 

to automatically fix the code style.

run

`npm run lint`

to check code style for all files.

run

`npm run lint -- --fix`

to fix the code style for all files

### With Prettier Hook 

No action needed, just do `git commit` and it should automatically format the code style for you.







