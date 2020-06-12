# A React Native Linter Guide with ESlint and Prettier

## Install from scratch

### ESlint

Install with 

`npm install eslint --save-dev`

Setup the configuration with 

`npx eslint --init`

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

`npx eslint yourfile.tsx`

to see the problem with current code style.

run 

`npx eslint yourfile.tsx --fix`

to automatically fix the code style.

### With Prettier Hook 

No action needed, just do `git commit` and it will automatically format the code style for you.







