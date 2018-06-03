# This is my dev/build process for static HTML pages.

It uses SASS & Autoprefixer. My examples use [YarnPKG](https://yarnpkg.com/lang/en/) you can use NPM if you want.

* yarn start
  * Runs live-server which creates a localhost environment watches all files in the directory
  * Reloads localhost when any files are edited.
  * I am running node-sass watch parallel to this to make it so my SASS changes are included in this reload.

* yarn build:css
  * Compiles my SASS to CSS
  * Runs Autoprefixer (post-css autoprefixer) on the CSS
  * Compresses the CSS