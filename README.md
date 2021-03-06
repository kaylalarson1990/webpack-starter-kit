# Webpack Starter Kit

## Fork This Repo

Within your group, decide on one person to have the project repository (repo) on their GitHub account. Then, that person should "fork" this repo. On the top right corner of this page, click the **Fork** button.

## Setup

After one person has forked the repo, everyone should clone down the forked repo. Since you don't want to name your project "webpack-starter-kit", you can use an optional argument when you run `git clone` (you replace the `[...]` with the terminal command arguments):

```bash
git clone [remote-address] [what you want to name the repo]
```

Once you have cloned the repo, install the library dependencies. Run:

```bash
npm install
```

To verify that it is setup correctly, run `npm start` in your terminal. Go to `http://localhost:8080/` and you should see a page with some `h1` text and a pink background. If that's the case, you're good to go. Enter `control + c` in your terminal to stop the server at any time.

## Where to Add Your Code

### JavaScript

You have to be very intentional with where you add your feature code. This repo uses a tool called [webpack](https://webpack.js.org/) to combine many JavaScript files into one big file. Webpack enables you to have many, separate JavaScript files to keep your code organized and readable. Webpack expects all of your code files to be in a specific place, or else it doesn't know how to combine them all behind the scenes.

**Create all of your feature code files in the `src` directory.**

Since code is separated into multiple files, you need to use the `import` and `export` syntax to share code across file.

Here is a video that walks through some information about [import and export](https://www.youtube.com/watch?v=_3oSWwapPKQ). There are a lot of resources out there about `import` and `export`, and resources will sometimes call them `ES6 modules`. It's something you will see in React and beyond.

### HTML

Add the HTML you need in the `index.html` file in the `./src` directory. There is some boilerplate HTML that exists from the start that you can modify.

### CSS (SCSS/SASS)

This project is setup to use SCSS/SASS files by default instead of your regular CSS files. Add your SCSS files in the `src/css` directory. There is a `base.scss` file already there, but you can change this file and add multiple SCSS files in this directory.

This might sound weird, but you need to `import` your SCSS files in the JavaScript entry file (`index.js`) for the styles to be applied to your HTML. The example `base.scss` file has already been imported in the JavaScript entry file as an example.

### Images

# Homescreen:
<img width="1494" alt="Screen Shot 2019-07-01 at 10 33 14 AM" src="https://user-images.githubusercontent.com/37026730/60452486-d5e9cd00-9beb-11e9-82cb-98020410bc8d.png">

# Search customer:
<img width="1633" alt="Screen Shot 2019-07-01 at 10 33 34 AM" src="https://user-images.githubusercontent.com/37026730/60452510-e39f5280-9beb-11e9-8003-8835fd84e824.png">

# Book a room:
<img width="1656" alt="Screen Shot 2019-07-01 at 10 33 43 AM" src="https://user-images.githubusercontent.com/37026730/60452513-e601ac80-9beb-11e9-920d-3b176b72b5d7.png">

# Search orders:
<img width="1660" alt="Screen Shot 2019-07-01 at 10 33 51 AM" src="https://user-images.githubusercontent.com/37026730/60452518-e8640680-9beb-11e9-977f-9e5cfe0b2fd2.png">


## How to View Your Code in Action

In the terminal, run:

```bash
npm start
```

You will see a bunch of lines output to your terminal. One of those lines will be something like:

```bash
Project is running at http://localhost:8080/
```

Go to `http://localhost:8080/` in your browser to view your code running in the browser.

---

## Test Files Organization

Similar to feature code, your test code needs to be put in a specific place for it to run successfully.

**Put all of your test files in the `test` directory.** As a convention, all test filenames should end with `-test.js`. For instance: `box-test.js`.

## Running Your Tests

Run your test suite using the command:

```bash
npm test
```

The test results will output to the terminal.

---

## Linting Your Code

Run the command in your terminal `npm run lint` to run the linter on your JavaScript code. There will be errors and warnings right from the start in this starter kit - the linter is still running successfully.

Your linter will look at the JavaScript files you have within the `src` directory and the `test` directory. 

## Webpack?

If you look in the `package.json` file, you'll see one of the library dependencies called `webpack`. If you're interested in learning more about what Webpack is and how it works behind the scenes, take a look through the [Webpack configuration documentation](https://webpack.js.org/concepts/).

## Deploying to GitHub Pages

_If you are finished with the functionality and testing of your project_, then you can consider deploying your project to the web! This way anyone can play it without cloning down your repo.

[GitHub Pages](https://pages.github.com/) is a great way to deploy your project to the web. Research deploying a Webpack project to GitHub Pages or ask your instructors about it if you get to that point. (Don't worry about this until your project is free of bugs and well tested!)
