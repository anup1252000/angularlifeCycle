# AngularlifeCycle

This project was generated with [Angular CLI](https://github.com/angular/angular-cli) version 12.1.2.


Hook method	Purpose	Timing
ngOnChanges()	
Respond when Angular sets or resets data-bound input properties. The method receives a SimpleChanges object of current and previous property values.

Note that this happens very frequently, so any operation you perform here impacts performance significantly. See details in Using change detection hooks in this document.

Called before ngOnInit() (if the component has bound inputs) and whenever one or more data-bound input properties change.

Note that if your component has no inputs or you use it without providing any inputs, the framework will not call ngOnChanges().

ngOnInit()	
Initialize the directive or component after Angular first displays the data-bound properties and sets the directive or component's input properties. See details in Initializing a component or directive in this document.

Called once, after the first ngOnChanges(). ngOnInit() is still called even when ngOnChanges() is not (which is the case when there are no template-bound inputs).

ngDoCheck()	
Detect and act upon changes that Angular can't or won't detect on its own. See details and example in Defining custom change detection in this document.

Called immediately after ngOnChanges() on every change detection run, and immediately after ngOnInit() on the first run.

ngAfterContentInit()	
Respond after Angular projects external content into the component's view, or into the view that a directive is in.

See details and example in Responding to changes in content in this document.

Called once after the first ngDoCheck().

ngAfterContentChecked()	
Respond after Angular checks the content projected into the directive or component.

See details and example in Responding to projected content changes in this document.

Called after ngAfterContentInit() and every subsequent ngDoCheck().

ngAfterViewInit()	
Respond after Angular initializes the component's views and child views, or the view that contains the directive.

See details and example in Responding to view changes in this document.

Called once after the first ngAfterContentChecked().

ngAfterViewChecked()	
Respond after Angular checks the component's views and child views, or the view that contains the directive.

Called after the ngAfterViewInit() and every subsequent ngAfterContentChecked().

ngOnDestroy()	
Cleanup just before Angular destroys the directive or component. Unsubscribe Observables and detach event handlers to avoid memory leaks. See details in Cleaning up on instance destruction in this document.

Called immediately before Angular destroys the direct

## Development server

Run `ng serve` for a dev server. Navigate to `http://localhost:4200/`. The app will automatically reload if you change any of the source files.

## Code scaffolding

Run `ng generate component component-name` to generate a new component. You can also use `ng generate directive|pipe|service|class|guard|interface|enum|module`.

## Build

Run `ng build` to build the project. The build artifacts will be stored in the `dist/` directory.

## Running unit tests

Run `ng test` to execute the unit tests via [Karma](https://karma-runner.github.io).

## Running end-to-end tests

Run `ng e2e` to execute the end-to-end tests via a platform of your choice. To use this command, you need to first add a package that implements end-to-end testing capabilities.

## Further help

To get more help on the Angular CLI use `ng help` or go check out the [Angular CLI Overview and Command Reference](https://angular.io/cli) page.
