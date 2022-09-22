# Brook. - A free and open source Eleventy 2 + Bootstrap 5 blog template

**Live Demo at**: <a href="https://templatedeck.com/" target="_blank">templatedeck.com</a>

## What is Brook?
Brook is a static HTML website template. Open sources and free to use.
It utilizes <a href="https://getbootstrap.com/" target="_blank">Bootstrap 5</a> and the the static site generator <a href="https://www.11ty.dev/" target="_blank">Eleventy</a> .

## How to use it as beginner
If you are familia with basic HTML but if you are not a web developer with advanced skills you can use Brook es well. Just use the `/public` folder of this repository. Change the content, add some of your images and transfer it to your webserver/webspace. Thats it

## How to use Brook if you have some advanced web development knowledge
Brook based on Bootstrap 5 and the static site generator Eleventy. It also comes with npm support for dependency management and Gulp as task runner.
In this setup I used the template language Nunjucks (by Mozilla) but Eleventy also supports Liquid, Handelbars, Haml, Pug, Mustach to name a few. Vanilla JS, static HTML or even Markdown files are also possible. It also lets you mix differend template languages together.
Eleventy also allows differend data types and ways to incorporate content during the deployment. You can use static and local content, compute content programatically, you can consume API´s, you can use the font matter format in files iteself, markdown content files etc.
Basically Brook is a all in on boilerplate for static websites + an example of design and layout.

## Requirements
You need Node (at least v14+) on your computer. To check if you have node and what version run this command in your terminal:
```
node --version
```

## Installation
Download and extract the [latest release](https://github.com/holger1411/11straps/releases) or checkout the main branch of this repo.
Fire up your terminal, go to the new folder and run:
```
npm install
```
Now you are good to go.

## Build it for dev
To build your static website for local development run:
```
npm run build-dev
```
This will build the static website into the `/dev` folder without all the minifiying and purging stuff (<- much faster and a more human friendly code output, but a much bigger package)

## Run in dev mode
To run the build-dev task automatically on file changes run:
```
npm run watch
```
That will run a local server from `/dev` folder and connects browser sync to it. On changes within the `/src` folder it will run the `npm run build-dev` command automatically and will refresh your browser.

## Build it for prod
If you are done with your dev work and happy with it its time to deploy your static website into the wild wild west (www). To build your static website for a prod deployment run:
```
npm run build
```
That will output the full site, with purged and minified CSS and minified html. The output will be stored in the `/public` folder. That folder is what you want to deploy to your webserver / hosting provider.
