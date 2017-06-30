# basescss
basescss is base SCSS for my new web project.


## Required

- node-sass
- node-sass-package-importer
- normalize.css
- postcss-cli
- autoprefixer
- csswring


## Get Started


Clone basescss.

    $ git clone git@github.com:42EG4M1/basescss.git [directory path]/src/scss


Install npm packages.

    $ npm i -D node-sass node-sass-package-importer postcss-cli autoprefixer csswring
    $ npm i -S normalize.css


Add the following to the package.json scripts.

    "scripts": {
      ･･･
      "build:sass": "node-sass --importer node_modules/node-sass-package-importer/dist/cli.js src/scss/all.scss dist/css/bundle.min.css",
      "build:postcss": "postcss dist/css/*.css --no-map --use autoprefixer -b \"last 2 versions\" --use csswring --output dist/css/*.css",
      "dev:sass": "node-sass --importer node_modules/node-sass-package-importer/dist/cli.js src/scss/all.scss dist/css/bundle.min.css --output-style expanded",
      "dev:postcss": "postcss dist/css/*.css --use autoprefixer -b \"last 2 versions\" --output dist/css/*.css",
      ･･･
    },


## commit message
    Fix    - Bug fixes.
    Add    - Add a new files and functions.
    Modify - Fixing features that are not bugs.
    Clean  - Organize by refactoring etc.
    Remove - Delete files.
    Rename - Rename files.
    Update - Update files.


## License
    MIT License
