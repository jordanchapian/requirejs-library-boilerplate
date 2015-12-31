# requirejs-library-boilerplate
Quickstart for building self-contained javascript libraries with requirejs. Prepackaged utilities, and grunt build system.

## Foundation

### Build system
The build system makes use of the Grunt task runner, and automates things such as documentation generation, test running, and source code builds.

### Auto-Documentation Generation
This boilerplate uses inline JSDoc comments by default. All of the boilerplate code provided in this repository is documented using JSDoc module format. To generate documentation for your project, use:

```bash
grunt explain
```

### Self Encapsulation via Almond.js
Using a start and end fragment, the library is contained in a self-executing anonymous function that exposes api points, and requires a base module. The boilerplate uses [Almond](https://github.com/jrburke/almond) as a replacement AMD loader for RequireJS. It provides a minimal AMD API footprint that includes loader plugin support. To build your project, use:

```bash
grunt default
```

### Modular unit / functional testing with Jasmine
Using [grunt-template-jasmine-requirejs](https://github.com/cloudchen/grunt-template-jasmine-requirejs), the boilerplate enables the programmer to specify the location of the specs, and use the requirejs describe syntax to specify the required modules for the tests. To run your tests, use:

```bash
grunt test
```
