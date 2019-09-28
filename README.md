# Angular8 Webpack Bundle Analyzer

<div align="center">
  <a href="https://github.com/webpack/webpack">
    <img width="200" height="200"
      src="https://webpack.js.org/assets/icon-square-big.svg">
  </a>
  <h1>Webpack Bundle Analyzer</h1>
  <p>Visualize size of webpack output files with an interactive zoomable treemap.</p>
</div>

## Why to use Webpack Bundle Analyzer in Angular 7/8 Application
This module will help you:

1. Realize what is *really* inside your bundle
2. Find out what modules make up the most of its size
3. Find modules that got there by mistake
4. Optimize it!

And the best thing is it supports minified bundles! It parses them to get real size of bundled modules.
And it also shows their gzipped sizes!

## What is Webpack Bundle Analyzer
Visualize size of webpack output files with an interactive zoomable treemap.

## How to Install
npm install --save-dev webpack-bundle-analyzer
npm install --save-dev webpack-cli

## How to Use it
1.run ng serve
2.ng build --statsJson=true
3.Add webpack-bundle-analyzer in script object in your angular 7/8 application package.json file
"scripts": {
    "ng": "ng",
    "start": "ng serve",
    "build": "ng build",
    "test": "ng test",
    "lint": "ng lint",
    "e2e": "ng e2e",
    "analyze":"webpack-bundle-analyzer dist/angular8-webpack-bundle-analyzer/stats-es2015.json"
  }
4.npm run analyze
5.This command will open a new browser window at port(http://127.0.0.1:8888/), and then you see your application budle utilization.

It will create an interactive treemap visualization of the contents of all your bundles.

![webpack bundle analyzer zoomable treemap](https://cloud.githubusercontent.com/assets/302213/20628702/93f72404-b338-11e6-92d4-9a365550a701.gif)

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 8.3.3.

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.


## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory. Use the `--prod` flag for a production build.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via [Protractor](http://www.protractortest.org/).

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI README](https://github.com/angular/angular-cli/blob/master/README.md).
