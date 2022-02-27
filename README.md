# Spoddify Mopped Plugin Template

This template can be used to create a Spoddify Mopped plugin.

## Use This Template

Click the link below to create a new GitHub Repository using this template, or click the _Use This Template_ button above.

#### [Create New Repository From Template](https://github.com/spoddify-mopped/spoddify-mopped-plugin-template/generate)

## Setup

Install all development node dependencies with:

```bash
npm install
```

## Update package.json

Edit the [`package.json`](package.json) and change the following values:

- `name`: This has to be prefixed with `spoddify-mopped-` or `@scope/spoddify-mopped-` to be recognized as valid plugin. It is not allowed to contain any spaces or special characters.
- `displayName`: This can be anything you want
- `description`: A short description about what your plugin does
- `repository.url`: Link to your repository
- `bugs.url`: Link to the issues page of your repository

## Build the plugin

This template uses TypeScript which needs to be compiled to JavaScript before it can be used. The following command will output the compilation to the `dist` directory:

```bash
npm run build
```

## Link to Spoddify Mopped

To test the plugin you can link the current directory to the global `node_modules`, so Spoddify Mopped can locate it:

```bash
npm link
```

Now start spoddify-mopped with:

```bash
spoddify-mopped -v
```

You should see a log message when your plugin was loaded successfully.

## Watch Changes

To auto-compile the code on changes, use:

```bash
npm run watch
```

> This will also restart spoddify-mopped for you. You have to stop any other running instance.
