# typhonjs-overview

In short <a href="https://typhonjs.io" target="_blank">TyphonJS / https://typhonjs.io</a> is a platform for modern mobile & web app development focusing not only on framework concerns, but also providing fully featured pipelines for integrated container deployment for server / database resources and web apps built on top of <a href="http://jspm.io/" target="_blank">JSPM</a> / <a href="https://github.com/systemjs/systemjs" target="_blank">SystemJS</a> including maintenance and monitoring solutions via <a href="https://coreos.com/rkt/" target="_blank">rkt</a> / <a href="http://kubernetes.io/" target="_blank">Kubernetes</a> / <a href="https://helm.sh/" target="_blank">Helm</a> facilitated by a standalone configuration / management app currently in development with local testing via <a href="https://github.com/TheNewNormal/kube-cluster-osx" target="_blank">Kube-Cluster macOS</a> or <a href="https://github.com/kubernetes/minikube" target="_blank">MiniKube</a> along with remote deployment. In addition for Javascript web apps integrated deployment options to convert them to desktop apps via <a href="http://electron.atom.io/" target="_blank">Electron</a> is available now and <a href="https://cordova.apache.org/" target="_blank">Cordova</a> for direct mobile deployment is forthcoming. 

TyphonJS provides a modernized version of Backbone / <a href="https://github.com/typhonjs-backbone/backbone-es6" target="_blank">backbone-es6</a> and related extensions for <a href="https://parse.com/" target="_blank">Parse</a> (<a href="https://github.com/typhonjs-backbone-parse/backbone-parse-es6" target="_blank">backbone-parse-es6</a>), <a href="https://www.firebase.com/" target="_blank">Firebase</a> (forthcoming), <a href="https://www.meteor.com/" target="_blank">Meteor</a> (halfway there) and <a href="http://www.socketstream.org/" target="_blank">SocketStream</a> (forthcoming). In addition a forthcoming complete data / event driven component library built on top of <a href="https://getmdl.io/" target="_blank">Material Design Lite</a> for backbone-es6 web apps is provided. However, the larger toolchain is applicable to any web app framework that can leverage JSPM / SystemJS. 

For native mobile apps TyphonJS provides a pipeline for container based deployment of server / database backends for cloud hosted solutions primarily Parse, Meteor and SocketStream. 

TyphonJS is a multi-organization / repo effort being open sourced under the <a href="https://www.mozilla.org/en-US/MPL/" target="_blank">MPLv2.0 license</a>. A multi org / repo toolchain is currently in development to support TyphonJS and beyond. This approach allows various modules / components of TyphonJS to be mixed and matched more easily with the web app framework of your choice amongst other scenarios. In many ways TyphonJS provides the glue between various important open source development / deployment tooling along with providing additional first party components. All first party Javascript source code is fully documented and is modern ES6 written in a standard idiomatic style. 

Please bear with us while the tooling and various framework integrations are completed. Full documentation and testing resources are already provided in most repos and a universal automated documentation repo / web site will be available soon. 

Below is an overview of all of the TyphonJS organizations / repos as of May 4th 2017. 

----------------

[typhonjs](https://github.com/typhonjs) - Provides common repos for TyphonJS

   - [typhonjs-overview](https://github.com/typhonjs/typhonjs-overview) - Provides an overview of TyphonJS.

[typhonjs-backbone](https://github.com/typhonjs-backbone)

   - [backbone-es6](https://github.com/typhonjs-backbone/backbone-es6) - A fork of Backbone converting it to ES6.
   - [typhonjs-core-backbone-common](https://github.com/typhonjs-backbone/typhonjs-core-backbone-common) - Provides the common TyphonJS extensions to Backbone-ES6
   - [typhonjs-core-backbone-events](https://github.com/typhonjs-backbone/typhonjs-core-backbone-events) - Separates 'events' support from Backbone in addition to adding TyphonJS extensions.
   - [typhonjs-core-backbone-events-logged](https://github.com/typhonjs-backbone/typhonjs-core-backbone-events-logged) - Provides a `typhonjs-core-logging` enabled version of `typhonjs-core-backbone-events`.
   - [typhonjs-core-backbone-localstorage](https://github.com/typhonjs-backbone/typhonjs-core-backbone-localstorage) - Provides a sync adapter using browser localStorage for backbone-es6.
   - [typhonjs-core-backbone-multistorage](https://github.com/typhonjs-backbone/typhonjs-core-backbone-multistorage) - Provides an adapter for backbone-es6 using typhonjs-core-multistorage.
   - [typhonjs-core-backbone-query](https://github.com/typhonjs-backbone/typhonjs-core-backbone-query) - A lightweight query API for Backbone Collections

[typhonjs-backbone-core](https://github.com/typhonjs-backbone-core) - Provides the core implementation of backbone-es6

[typhonjs-backbone-esnext](https://github.com/typhonjs-backbone-esnext) - Provides a version of Backbone meant to be used with ES6+

   - [backbone-esnext-eventbus](https://github.com/typhonjs-backbone-esnext/backbone-esnext-eventbus) - Provides a default main eventbus instance for backbone-esnext-events.
   - [backbone-esnext-events](https://github.com/typhonjs-backbone-esnext/backbone-esnext-events) - Provides enhanced Backbone events functionality.

[typhonjs-backbone-firebase](https://github.com/typhonjs-backbone-firebase) - Forthcoming typhonjs-backbone support for Firebase

[typhonjs-backbone-parse](https://github.com/typhonjs-backbone-parse) - Provides support for Parse for typhonjs-backbone

   - [backbone-parse-es6](https://github.com/typhonjs-backbone-parse/backbone-parse-es6) - A fork of Backbone converting it to ES6 along with Parse 1.6+ integration and ES5 bundles.
   - [typhonjs-core-parse](https://github.com/typhonjs-backbone-parse/typhonjs-core-parse)
   - [typhonjs-core-parse-init](https://github.com/typhonjs-backbone-parse/typhonjs-core-parse-init)
   - [typhonjs-core-parse-user](https://github.com/typhonjs-backbone-parse/typhonjs-core-parse-user)

[typhonjs-browser](https://github.com/typhonjs-browser) - Provides browser specific utilities and modules.

   - [zepto](https://github.com/typhonjs-browser/zepto) - Zepto.js is a minimalist JavaScript library for modern browsers, with a jQuery-compatible API and mods for consumption in JSPM

[typhonjs-common](https://github.com/typhonjs-common) - Provides common isometric modules / components that run on the server & client.

   - [typhonjs-core-collections](https://github.com/typhonjs-common/typhonjs-core-collections) - Provides several collection oriented data structures. 
   - [typhonjs-core-logging](https://github.com/typhonjs-common/typhonjs-core-logging) - Provides a pluggable logging module for universal logging across TyphonJS repos. 
   - [typhonjs-core-logging-socket](https://github.com/typhonjs-common/typhonjs-core-logging-socket) - Provides a logging plugin for typhonjs-core-logging that sends data over a WebSocket or SockJS.
   - [typhonjs-core-multistorage](https://github.com/typhonjs-common/typhonjs-core-multistorage) - Provides basic platform independent storage.
   - [typhonjs-core-socket](https://github.com/typhonjs-common/typhonjs-core-socket) - Provides a default socket implementation supporting WebSockets and sock.js
   - [typhonjs-core-utils](https://github.com/typhonjs-common/typhonjs-core-utils) - Provides common utility functionality.

[typhonjs-demos](https://github.com/typhonjs-demos) - Provides demos for all TyphonJS repos.

   - [backbone-es6-localstorage-todos](https://github.com/typhonjs-demos/backbone-es6-localstorage-todos) - Provides the canonical TODOs demo for backbone-es6 and typhonjs-core-backbone-localstorage w/ JSPM & SystemJS.
   - [backbone-es6-localstorage-todos-global-es5](https://github.com/typhonjs-demos/backbone-es6-localstorage-todos-global-es5) - Provides the canonical TODOs demo for backbone-es6 using the ES5 global bundle (backbone.js)
   - [backbone-es6-localstorage-todos-requirejs-es5](https://github.com/typhonjs-demos/backbone-es6-localstorage-todos-requirejs-es5) - Provides the canonical TODOS web app using RequireJS and the AMD ES5 bundle generated by backbone-es6 and typhonjs-core-backbone-localstorage.
   - [backbone-parse-es6-todos](https://github.com/typhonjs-demos/backbone-parse-es6-todos) - Provides the canonical TODOs demo for backbone-parse-es6 and JSPM / SystemJS.
   - [backbone-parse-es6-todos-global-es5](https://github.com/typhonjs-demos/backbone-parse-es6-todos-global-es5) - Provides the canonical TODOs demo for backbone-parse-es6 using the ES5 global bundle (backbone-parse.js)
   - [backbone-parse-es6-todos-improved](https://github.com/typhonjs-demos/backbone-parse-es6-todos-improved) - Provides the canonical TODOs app for backbone-parse-es6 showing improved with TyphonJS functionality.
   - [backbone-parse-es6-todos-requirejs-es5](https://github.com/typhonjs-demos/backbone-parse-es6-todos-requirejs-es5) - Provides the canonical TODOS web app using RequireJS and the AMD ES5 bundle generated by backbone-parse-es6.

[typhonjs-demos-deploy-electron](https://github.com/typhonjs-demos-deploy-electron) - Creates desktop apps using Electron from typhonjs-demos

   - [electron-backbone-es6-localstorage-todos](https://github.com/typhonjs-demos-deploy-electron/electron-backbone-es6-localstorage-todos) - Creates a desktop app  from backbone-es6-localstorage-todos using Electron.
   - [electron-backbone-parse-es6-todos-improved](https://github.com/typhonjs-demos-deploy-electron/electron-backbone-parse-es6-todos-improved) - Creates a desktop app from backbone-parse-es6-todos-improved using Electron.

[typhonjs-demos-test](https://github.com/typhonjs-demos-test) - Provides testing repos specific to issues related to TyphonJS.

   - [istanbul-jspm-coverage-example](https://github.com/typhonjs-demos-test/istanbul-jspm-coverage-example) - Provides an example of instrumenting JSPM / SystemJS for code coverage with Istanbul / Mocha.
   - [typhonjs-issues-demos](https://github.com/typhonjs-demos-test/typhonjs-issues-demos) - Provides various demos for issues raised with all TyphonJS repos.

[typhonjs-governance](https://github.com/typhonjs-governance) - Provides all versioned docs, specs, and governance repos. 

   - [typhonjs-core-docs](https://github.com/typhonjs-governance/typhonjs-core-docs) - Provides overview documentation for all TyphonJS orgs / repos.
   - [typhonjs-core-governance](https://github.com/typhonjs-governance/typhonjs-core-governance) - Provides the authoritative documentation regarding TyphonJS governance.
   - [typhonjs-core-specifications](https://github.com/typhonjs-governance/typhonjs-core-specifications) - Provides overview documentation for all TyphonJS orgs / repos.

[typhonjs-meteor-ddp-client](https://github.com/typhonjs-meteor-ddp-client) - Provides a generic client for DDP (Distributed Data Protocol) and plugin mechanism to link to MVC libraries.

   - [backbone-meteor-es6](https://github.com/typhonjs-meteor-ddp-client/backbone-meteor-es6)
   - [typhonjs-core-asteroid](https://github.com/typhonjs-meteor-ddp-client/typhonjs-core-asteroid) - An ES6 fork of Asteroid providing a generic client for Meteor. 
   - [typhonjs-core-asteroid-belt](https://github.com/typhonjs-meteor-ddp-client/typhonjs-core-asteroid-belt) - Wouldn't you like to know.... coming soon... :D
   - [typhonjs-core-asteroid-init](https://github.com/typhonjs-meteor-ddp-client/typhonjs-core-asteroid-init)
   - [typhonjs-core-socket-ddp](https://github.com/typhonjs-meteor-ddp-client/typhonjs-core-socket-ddp) - Provides a Javascript DDP client

[typhonjs-node-ast](https://github.com/typhonjs-node-ast) - Provides utility NPM modules for working with Javascript / AST.

   - [typhonjs-ast-walker](https://github.com/typhonjs-node-ast/typhonjs-ast-walker) - Provides a simple Javascript AST traversal utility that traverses all nodes / children regardless of type.

[typhonjs-node-config](https://github.com/typhonjs-node-config) - Provides utility NPM modules for configuration data.

   - [typhonjs-config-eslint](https://github.com/typhonjs-node-config/typhonjs-config-eslint) - Provides shared ESLint configs for TyphonJS repos.

[typhonjs-node-escomplex](https://github.com/typhonjs-node-escomplex) - Next generation complexity reporting for Javascript based on babylon, but supporting all major AST generators.

   - [escomplex-plugin-analyze-threshold](https://github.com/typhonjs-node-escomplex/escomplex-plugin-analyze-threshold) - Provides project and module oriented threshold analysis for typhonjs-escomplex complexity reports.
   - [escomplex-plugin-formats-xml](https://github.com/typhonjs-node-escomplex/escomplex-plugin-formats-xml) - Provides a plugin for typhonjs-escomplex project result / module report transformation to XML.
   - [escomplex-plugin-metrics-module](https://github.com/typhonjs-node-escomplex/escomplex-plugin-metrics-module) - Provides the core module metric / report generation plugin for typhonjs-escomplex module processing.
   - [escomplex-plugin-metrics-project](https://github.com/typhonjs-node-escomplex/escomplex-plugin-metrics-project) - Provides the core project metric / report generation plugin for typhonjs-escomplex project processing.
   - [escomplex-plugin-syntax-babylon](https://github.com/typhonjs-node-escomplex/escomplex-plugin-syntax-babylon) - Provides a plugin for typhonjs-escomplex module processing which loads syntax definitions for trait resolution for Babylon AST.
   - [escomplex-plugin-syntax-estree](https://github.com/typhonjs-node-escomplex/escomplex-plugin-syntax-estree) - Provides a plugin for typhonjs-escomplex module processing which loads syntax definitions for trait resolution for ESTree AST.
   - [plato](https://github.com/typhonjs-node-escomplex/plato) - JavaScript source code visualization, static analysis, and complexity tool
   - [typhonjs-escomplex](https://github.com/typhonjs-node-escomplex/typhonjs-escomplex) - Next generation complexity reporting for Javascript based on babylon.
   - [typhonjs-escomplex-analyze](https://github.com/typhonjs-node-escomplex/typhonjs-escomplex-analyze) - Provides project and module oriented analysis for typhonjs-escomplex complexity reports.
   - [typhonjs-escomplex-commons](https://github.com/typhonjs-node-escomplex/typhonjs-escomplex-commons) - Provides core common utilities for typhonjs-escomplex plugins including trait resolution.
   - [typhonjs-escomplex-module](https://github.com/typhonjs-node-escomplex/typhonjs-escomplex-module) - Provides module / individual file oriented AST processing for typhonjs-escomplex complexity reports.
   - [typhonjs-escomplex-project](https://github.com/typhonjs-node-escomplex/typhonjs-escomplex-project) - Provides project oriented AST processing for typhonjs-escomplex complexity reports.
   - [typhonjs-escomplex-test-data](https://github.com/typhonjs-node-escomplex/typhonjs-escomplex-test-data) - Provides shared test data resources for all typhonjs-escomplex repos.

[typhonjs-node-esdoc](https://github.com/typhonjs-node-esdoc) - Provides NPM modules for ESDoc plugins.

   - [esdoc](https://github.com/typhonjs-node-esdoc/esdoc) - A maintained fork of ESDoc - good documentation for JavaScript(ES2015)
   - [esdoc-plugin-dependency-graphs](https://github.com/typhonjs-node-esdoc/esdoc-plugin-dependency-graphs) - A plugin for ESDoc that adds interactive D3 powered dependency graphs for source code including linking JSPM / NPM managed code and packages.
   - [esdoc-plugin-enhanced-navigation](https://github.com/typhonjs-node-esdoc/esdoc-plugin-enhanced-navigation) - Replaces the standard ESDoc left hand source navigation with an enhanced version. 
   - [esdoc-plugin-escomplex](https://github.com/typhonjs-node-esdoc/esdoc-plugin-escomplex) - A plugin for ESDoc that produces complexity analysis reports via escomplex.
   - [esdoc-plugin-extends-replace](https://github.com/typhonjs-node-esdoc/esdoc-plugin-extends-replace) - An ESDoc plugin to replace unconnected "extends" tags w/ actual class references.
   - [esdoc-plugin-jspm](https://github.com/typhonjs-node-esdoc/esdoc-plugin-jspm) - A plugin for ESDoc that enables end to end documentation linking JSPM / SystemJS managed packages in addition to a source root. 
   - [esdoc-plugin-npm](https://github.com/typhonjs-node-esdoc/esdoc-plugin-npm) - A plugin for ESDoc that enables end to end documentation linking NPM managed packages in addition to a source root.
   - [typhonjs-node-esdoc](https://github.com/typhonjs-node-esdoc/typhonjs-node-esdoc) - Provides a NPM module combining ESDoc with all plugins available.

[typhonjs-node-gulp](https://github.com/typhonjs-node-gulp) - Provides NPM modules for various Gulp tasks.

   - [typhonjs-core-gulptasks](https://github.com/typhonjs-node-gulp/typhonjs-core-gulptasks) - Provides common gulp tasks shared by TyphonJS and beyond for JSPM / SystemJS projects.
   - [typhonjs-github-orgs-gulptasks](https://github.com/typhonjs-node-gulp/typhonjs-github-orgs-gulptasks) - Provides GitHub many organization / repos gulp tasks shared by TyphonJS and beyond.

[typhonjs-node-jspm](https://github.com/typhonjs-node-jspm) - Provides utility NPM modules for interfacing with JSPM / SystemJS.

   - [typhonjs-config-jspm-parse](https://github.com/typhonjs-node-jspm/typhonjs-config-jspm-parse) - Provides a NPM module to parse dependencies from JSPM entries in `package.json` and `config.js` via an instance of SystemJS / SystemJS Loader.
   - [typhonjs-istanbul-instrument-jspm](https://github.com/typhonjs-node-jspm/typhonjs-istanbul-instrument-jspm) - Provides a NPM module to add Istanbul instrumentation to JSPM / SystemJS by replacing the System.translate hook. 

[typhonjs-node-npm-scripts](https://github.com/typhonjs-node-npm-scripts) - Provides various NPM modules / scripts including build / testing modules.

   - [typhonjs-npm-build-test](https://github.com/typhonjs-node-npm-scripts/typhonjs-npm-build-test) - Provides a unified set of NPM scripts and dependencies for building and testing ES6+ NPM modules for TyphonJS and beyond.
   - [typhonjs-npm-scripts-build-babel](https://github.com/typhonjs-node-npm-scripts/typhonjs-npm-scripts-build-babel) - Provides NPM scripts for building ES6+ projects using Babel for all TyphonJS NPM modules and beyond.
   - [typhonjs-npm-scripts-publish](https://github.com/typhonjs-node-npm-scripts/typhonjs-npm-scripts-publish) - Provides NPM scripts for pre-publish & publish actions for TyphonJS NPM modules and beyond.
   - [typhonjs-npm-scripts-runner](https://github.com/typhonjs-node-npm-scripts/typhonjs-npm-scripts-runner) - Provides an NPM module and script which will load a JSON file searching for an Array entry then executes the scripts. 
   - [typhonjs-npm-scripts-test-mocha](https://github.com/typhonjs-node-npm-scripts/typhonjs-npm-scripts-test-mocha) - Provides NPM scripts for testing projects using Istanbul & Mocha for all TyphonJS NPM modules and beyond.

[typhonjs-node-plugin](https://github.com/typhonjs-node-plugin) - Provides a generic plugin infrastructure

   - [typhonjs-plugin-loader](https://github.com/typhonjs-node-plugin/typhonjs-plugin-loader) - Provides generic plugin loading from installed node modules or directly from the file system.
   - [typhonjs-plugin-manager](https://github.com/typhonjs-node-plugin/typhonjs-plugin-manager) - Provides a plugin manager that dispatches events to loaded plugins.

[typhonjs-node-scm](https://github.com/typhonjs-node-scm) - Provides utility NPM modules for interfacing with source code management systems.

   - [typhonjs-github-inspect-orgs](https://github.com/typhonjs-node-scm/typhonjs-github-inspect-orgs) - A NPM module providing compound GitHub queries spanning multiple organizations / users for many-repo projects such as TyphonJS.
   - [typhonjs-github-inspect-orgs-transform](https://github.com/typhonjs-node-scm/typhonjs-github-inspect-orgs-transform) - Provides a NPM module that transforms data from typhonjs-github-inspect-orgs to normalized HTML, markdown, JSON or text.

[typhonjs-node-tjsdoc](https://github.com/typhonjs-node-tjsdoc) - Provides a modern JS documentation system for ES6+ & Typescript.

   - [tjsdoc](https://github.com/typhonjs-node-tjsdoc/tjsdoc) - Provides common orchestration for TJSDoc.
   - [tjsdoc-babylon](https://github.com/typhonjs-node-tjsdoc/tjsdoc-babylon) - Provides Babylon / ES6+ documentation generation for Javascript.
   - [tjsdoc-docs-babylon](https://github.com/typhonjs-node-tjsdoc/tjsdoc-docs-babylon) - Provides Babylon doc tag generation for TJSDoc.
   - [tjsdoc-docs-common](https://github.com/typhonjs-node-tjsdoc/tjsdoc-docs-common) - Provides common doc tag generation for TJSDoc.
   - [tjsdoc-docs-typescript](https://github.com/typhonjs-node-tjsdoc/tjsdoc-docs-typescript) - Provides Typescript doc tag generation for TJSDoc.
   - [tjsdoc-publisher-static-html](https://github.com/typhonjs-node-tjsdoc/tjsdoc-publisher-static-html) - Provides a publishing module for TJSDoc generating static HTML documentation.
   - [tjsdoc-runtime-common](https://github.com/typhonjs-node-tjsdoc/tjsdoc-runtime-common) - Provides the common shared runtime for TJSdoc.
   - [tjsdoc-test-utils](https://github.com/typhonjs-node-tjsdoc/tjsdoc-test-utils) - Provides common testing utilities for tjsdoc (non-published)
   - [tjsdoc-tests-ecmascript](https://github.com/typhonjs-node-tjsdoc/tjsdoc-tests-ecmascript) - Provides shared Javascript testing resources for TJSDoc utilized across various repos.
   - [tjsdoc-typescript](https://github.com/typhonjs-node-tjsdoc/tjsdoc-typescript) - Forthcoming documentation generation for Typescript.

[typhonjs-node-tjsdoc-plugins](https://github.com/typhonjs-node-tjsdoc-plugins) - Provides officially supported TJSDoc plugins.

   - [tjsdoc-plugin-dependency-graphs](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-dependency-graphs) - A plugin for TJSDoc that adds interactive D3 powered dependency graphs for source code including linking JSPM / NPM managed code and packages.
   - [tjsdoc-plugin-escomplex](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-escomplex) - A forthcoming plugin for TJSDoc that produces complexity analysis reports via typhonjs-escomplex.
   - [tjsdoc-plugin-external-ecmascript](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-external-ecmascript) - Provides built-in external references for ECMAScript.
   - [tjsdoc-plugin-external-nodeapi](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-external-nodeapi) - Provides forthcoming built-in external references for the Node API.
   - [tjsdoc-plugin-external-webapi](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-external-webapi) - Provides built-in external references for the web API.
   - [tjsdoc-plugin-jspm](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-jspm) - A plugin for TJSDoc that enables end to end documentation linking JSPM / SystemJS managed packages in addition to a source root.
   - [tjsdoc-plugin-live-server](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-live-server) - Provides a plugin that starts `live-server` providing refresh of the output doc target during TJSDoc execution.
   - [tjsdoc-plugin-npm](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-npm) - A plugin for TJSDoc that enables end to end documentation linking NPM managed packages in addition to a source root.
   - [tjsdoc-plugin-watcher](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-watcher) - Provides file watching control and event bindings which other plugins may consume.
   - [tjsdoc-plugin-watcher-doc-regenerate](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-watcher-doc-regenerate) - Provides incremental doc regeneration utilizing typhonjs-plugin-watcher.
   - [tjsdoc-plugin-webpack](https://github.com/typhonjs-node-tjsdoc-plugins/tjsdoc-plugin-webpack) - A forthcoming plugin for TJSDoc that enables end to end documentation linking Webpack managed packages in addition to local source roots.

[typhonjs-node-utils](https://github.com/typhonjs-node-utils) - Provides various utility NPM modules 

   - [typhonjs-color-logger](https://github.com/typhonjs-node-utils/typhonjs-color-logger) - Provides ANSI color logging.
   - [typhonjs-config-resolver](https://github.com/typhonjs-node-utils/typhonjs-config-resolver) - Provides support to load config files and local or module extensions along with validation.
   - [typhonjs-config-resolver-tests](https://github.com/typhonjs-node-utils/typhonjs-config-resolver-tests) - Provides test data for typhonjs-config-resolver as an NPM module.
   - [typhonjs-file-util](https://github.com/typhonjs-node-utils/typhonjs-file-util) - Provides several utility methods for archiving, copying, reading, and writing files.
   - [typhonjs-ice-cap](https://github.com/typhonjs-node-utils/typhonjs-ice-cap) - Programmable DOM-based HTML template library.
   - [typhonjs-live-server](https://github.com/typhonjs-node-utils/typhonjs-live-server) - Provides a plugin wrapping `live-server` adding event bindings and workarounds for graceful shutdown.
   - [typhonjs-object-util](https://github.com/typhonjs-node-utils/typhonjs-object-util) - Provides common object manipulation utilities.
   - [typhonjs-package-util](https://github.com/typhonjs-node-utils/typhonjs-package-util) - Provides several utility methods for working with `package.json`.
   - [typhonjs-path-resolver](https://github.com/typhonjs-node-utils/typhonjs-path-resolver) - Provides utility methods to resolve file paths relative to a given location and package name.

[typhonjs-socketstream-client](https://github.com/typhonjs-socketstream-client) - Provides a generic client for SocketStream and plugin mechanism to link to MVC libraries.

[typhonjs-utils](https://github.com/typhonjs-utils) - Provides miscellaneous utility repos.

   - [intellij-plugin-jspm](https://github.com/typhonjs-utils/intellij-plugin-jspm) - Provides JSPM reference and path completion plugin for WebStorm, PHPStorm and other Idea family IDE supporting Javascript.

[typhonjs-websites](https://github.com/typhonjs-websites) - Provides several web site resources for TyphonJS

   - [docs.typhonjs.io](https://github.com/typhonjs-websites/docs.typhonjs.io) - Provides documentation for all TyphonJS repos.
   - [typhonjs.io](https://github.com/typhonjs-websites/typhonjs.io) - The main TyphonJS website... 

[typhonjs-zenhub](https://github.com/typhonjs-zenhub) - Provides a common location for all ZenHub projects tracking all repos from each major TyphonJS org category. 

   - [zenhub-typhonjs](https://github.com/typhonjs-zenhub/zenhub-typhonjs) - Provides a ZenHub overview of all TyphonJS orgs / repos.

