# SASS practice
Here is a bare-bones project using SASS, with auto-watching of changes to SASS files. 

## Usage

run `npm install`, which will install the [node-sass library](https://www.npmjs.com/package/node-sass). 

In one terminal, run `lite-server` to get the basic server going to serve the page.

In other terminal, run `npm run scss` (look at the "scripts" in the package.json to see what that runs) and it will look for changes (saves) to .scss files inside of assets/scss and compile it to a single file at assets/css/styles.css. 

So why don't the numerous .scss files compile into numerous .css files? That's because the files in the scss folder with an underscore are called "partials," which then get imported into styles.scss. 

That styles.scss file only has imports in it - everything else is declared in those partials. 