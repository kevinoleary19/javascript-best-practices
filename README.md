# Javascript Best Practices

- Immutability

- Composition over Inheritence

- Unidirectional data flow

- single source of truth

- unidirectional data flow
- smaller component files (large components with multiple render methods conflates business logic and makes it hard to map imports / logic to corresponding view layers)
- globals are a spawn of satan
- use attributes instead of static getters. getters are good for hiding side effects and business logic, but unneccesary for returning strings. services should be close to back end apis; exposing explicit methods
- Static Type Checking

### Data retrieval
- fetch (downside is that they are not cancellable)

### es6
- destructuring
- promises
- generators (never used personally, but cool nevertheless)

### es7
- async await
- observables (rxjs as reliable implementation)
- decorators (as of right now there is no standard and they are in an early stage, so it's risky to use. HOCs are comparable and easier to test)

### Tooling

- Webpack (Tree shaking, code splitting, base64 image conversion, extensive plugins, community support, Hot module reloading)
- eslint
- yarn for dependency management and intelligent module versioning

### CSS
- z-index scale
- reused components should recieve special styling through a wrapper div within a parent
- don't use scss `extend`. Use `mixins` [instead](https://www.sitepoint.com/avoid-sass-extend/).
