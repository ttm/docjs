# jsdoc boilerplate
For usage with jardim.in

## file structure of the package
The doc/ folder has the configuration script for jsdoc and
the executable to create the HTML from the source files.
It reads components/ and pages/ and outputs the HTML files in
doc/out/ folder.

## usage
Enter doc/ folder and run the ./runme.sh script.
It will render ./out using jsdoc.

## workings
Every .vue and .js files inside the folders are parsed, recursively.
Comments come before the function or class, or in a file, with two stars,
as in:

    /**
    *
    *
    */

# documentation generators for javascript
jsdoc is somewhat the standard and are used for many other documentation generators. It really seems to be able to do all we want.
Thus we start with it.

## about jsdoc
There are inline and block comments and they work differently for jsdoc.
You can trigger events by using special tokens in comments (such as @).
Block comments have usual documentation (e.g. name, description,
variable types and description), and come before the function.

Generated HTML is of good quality and navigates from the objects to the
source files.

### events and handlers
Tokens are used as events, or event triggers.
Handlers are functions inside .... file.

## alternatives

https://github.com/documentationjs/documentation#documentation

https://sphinx-js-howto.readthedocs.io/en/latest/

https://github.com/slatedocs/slate
(tem p js e vimL)

### for vue
https://github.com/Kocal/jsdoc-vuejs

#### vuese 
https://dev.to/berniwittmann/quick--easy-documentation-generation-for-vuejs-components-7k6

need to install tslint:
    $ yarn global add tslint typescript

then 
1. clone repo: https://github.com/vue-contrib/vuese
2. cd vuese
3. yarn install
4. yarn run build
5. yarn link

In the project you want to make de documentation files:
1. If @vuese/cli is not yet installed, add it: yarn add @vuese/cli
2. Run yarn link vuese-monorepo
3. Navigate to node_modules/.bin and open vuese.cmd and vuese
4. Change any instance of @vuese to vuese-monorepo\packages in both files
5. Run node_modules/.bin/vuese gen



#### único que vi fazendo tudo com simples //
http://ashkenas.com/docco/
