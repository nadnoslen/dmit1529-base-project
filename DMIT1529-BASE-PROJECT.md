# dmit1529-base-project

This is a basic html+css+js base project. Use a copy of it to create all your new local web page projects.

## Why - What Is So Special?

Here's a summary of what makes this project special:

- ✅ It places all code inside a `src` directory -> get used to it
- ✅ It has been initialised as a git repository -> this will make more sense later in life
- ✅ It has an HTMLHint configuration file (`.htmlhintrc`) ->
- ✅ It has a StyleLint configuration file (`.stylelintrc.json`)
- ✅ It has a Prettier configuration file ()

## Getting Started

### Requirements

- [Node.js](https://nodejs.org/)

To get all of the VS Code features to work, you must install the NPM packages that perform the linting and formatting of your projects files.

Execute the following command from the root of your project.

```shell
npm install
```

### VS Code Extensions

Several extensions are recommended by this project. You will be prompted to install them when you first open the project in VS Code.

You can always visit the Extension panel and search for `@recommended` to see the list of **WORKSPACE RECOMMENDATIONS**. Installing these will give you the ultimate developer experience.

**These extension are terrific because they give you instant feedback in your editor when you've violated a rule.**

### Running Prettier

Prettier is a code formatter for your project.

This project explicitly tells VS Code:

1. Format files with Prettier.
1. Format your files automatically when you save.
1. Save will a slight delay if you leave the VS Code app or visit another file.

#### Running Prettier Script

````shell
# reports the files that need to be re-formatted
npm run-script prettier:check

# formats all files in the project (if they need it)
npm run-script prettier:write
```

### Running The Static Analysis Scripts Individually

```shell
# static analysis of your css file(s)
npm run-script lint:css

# static analysis of your html file(s)
npm run-script lint:html

# static analysis of your javascript file(s)
npm run-script lint:js
````

### Running ALL Static Analysis Scripts Concurrently

```shell
# runs static analysis of css/html/javascript all at the same time!
npm run-script lint
```

## Static Analysis Tools

### ESLint

Javascript static analysis. Makes sure you have't declared any unused variables, left console logging in your code, etc.

Check out the rules reference here: https://eslint.org/docs/latest/rules/

You can configure rules for your project in the `eslint.config.mjs` file.

### HTMLHint

HTML static analysis. Makes sure your HTML is compliant, tags are closed, attributes are not duplicated, etc.

Check out the rules reference here: https://htmlhint.com/docs/user-guide/list-rules

You can configure rules for your project in the `.htmlhintrc` file.

### Stylelint

CSS static analysis. Helps avoid common errors in your style definitions.

Check out the rules reference here: https://stylelint.io/user-guide/rules

You can configure rules for your project in the `.stylelintrc.yml` file.

## Code Formatting

### Prettier

An opinionated code formatter.
