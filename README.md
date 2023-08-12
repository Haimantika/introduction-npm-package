# Creating Your Own NPX Introduction Command

Creating your own `npx` introduction command can be a fun and useful project! The `npx` command allows you to run Node.js-based packages without having to globally install them. Here's a step-by-step guide to creating your own `npx` introduction command:

## Step 1: Choose a Package Name

Decide on a unique name for your package. This name will be used to invoke your introduction command using `npx`.

## Step 2: Create a New Directory

Create a new directory for your package. You can name it after the package name you chose in the previous step.

```bash
mkdir my-npx-intro
cd my-npx-intro
```

## Step 3: Initialize Your Package

Initialize your project as a Node.js package using the following command:
```bash
npm init -y
```

## Create an Executable Script:
Inside your project directory, create a JavaScript file that will serve as the executable script for your npx command. Let's call this file index.js. You can follow my example or edit it accordingly.

### Make sure to define bin in 'package.json'
```json
"bin": {
  "my-npx-command": "./index.js"
},
```
## Make the Script Executable:
In your terminal, make your script file executable by running:

```bash
chmod +x index.js
```

## Test your command
- Link the package using `npm link`
- Test by running the command `npx package-name`
- If it works as expected, make sure to unlink it using `npm unlink -g directory-name`

## Publish your package
- Make an [npm account](https://www.npmjs.com/) 
- Login to your account using the command `npm login`
- Publish the package using the command `npm publish`

Send it to your friends and find a cool way to introduce yourself!
