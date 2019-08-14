# AngularLifecycleDemo

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 7.2.3.

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


Lifecycle Hooks
### ngOnChanges()
    Used in pretty much any component that has an input.
    Called whenever an input value changes
    Is called the first time before ngOnInit

### ngOnInit()
    Used to initialize data in a component.
    Called after input values are set when a component is initialized.
    Added to every component by default by the Angular CLI.
    Called only once

### ngDoCheck()
    Called during all change detection runs
    A run through the view by Angular to update/detect changes

### ngAfterContentInit()
    Called only once after first ngDoCheck()
    Called after the first run through of initializing content'

### ngAfterContentChecked()
    Called after every ngDoCheck()
    Waits till after ngAfterContentInit() on first run through

### ngAfterViewInit()
    Called after Angular initializes component and child component content.
    Called only once after view is initialized

### ngAfterViewChecked()
    Called after all the content is initialized and checked. (Component and child components).
    First call is after ngAfterViewInit()
    Called after every ngAfterContentChecked() call is completed

### ngOnDestroy()
    Used to clean up any necessary code when a component is removed from the DOM.
    Fairly often used to unsubscribe from things like services.
    Called only once just before component is removed from the DOM.