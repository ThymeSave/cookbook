# Silverware

Silverware is the hart of ThymeSave.

It contains most of the logic, party split into separate packages allowing easier modularization:

| Package                 | Scope                                               |
|:------------------------|:----------------------------------------------------|
| @thymesave/core         | models, API definitions                             |
| @thymesave/translations | translations and matching functionality             |
| @thymesave/ingredients  | ingredient parsing, mapping and definitions         |
| @thymesave/plugin       | Plugin functionality for extending ThymeSave easily |

The frontend is completely written in TypeScript and Angular.

## Why Angular?

Angular is a battle proven framework we use it in combination with Angular Material, which provides great accessibility
and a few handy components out of the box.

Also, with Material Design we already have a design system that works and don't have to reinvent the wheel.

To round the angular toolbox also Angular Flex is used, providing Flexbox layouts via directives.

## Basic concepts / ideology

- Don't cache database stuff explicitly
    - PouchDB is used as storage layer which gives great performance with IndexedDB
    - A store layer is explicitly not added, reducing complexity and possible points of failures
- The npm packages
    - are as loosely coupled as possible
    - have high test coverage, covering also most edge cases
- The angular part
    - contains test where it adds value, we don't have a coverage goal here (yet)
    - is split into components where suitable
    - utilizes best practices where ever it makes sense, we keep it open to make own design decisions that might not be
      compliant with "the angular way"
- We use observables (RxJS) and TypeScript features where ever possible
    - promises are just used e.g. in plugins to make the entry easier for plugin developers OR if not otherwise possible

## Further resources

- [Angular](https://angular.io)
- [Angular Material](https://material.angular.io/)
- [Angular Flex](https://github.com/angular/flex-layout)
- [PouchDB](https://pouchdb.com/)
- [RxJS](https://rxjs.dev/)
- [GitHub repository](https://github.com/thymesave/silverware)
