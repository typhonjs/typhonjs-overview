# typhonjs-overview

In short TyphonJS is a platform for modern mobile & web app development focusing not only on framework concerns, but also providing fully featured pipelines for integrated container deployment for server / database resources and web apps built on top of JSPM / SystemJS including maintenance and monitoring solutions via <a href="https://coreos.com/rkt/" target="_blank">rkt</a> / <a href="http://kubernetes.io/" target="_blank">Kubernetes</a> / <a href="http://rancher.com/" target="_blank">Rancher</a>. In addition for Javascript web apps integrated deployment options to convert them to desktop apps via Electron is available now and Cordova for direct mobile deployment is forthcoming. 

TyphonJS provides a modernized version of Backbone / [backbone-es6](https://github.com/typhonjs-backbone/backbone-es6) and related extensions for Parse ([backbone-parse-es6](https://github.com/typhonjs-backbone-parse/backbone-parse-es6)), Firebase (forthcoming), Meteor (halfway there) and SocketStream (forthcoming). In addition a forthcoming complete component library for building Material Design web apps is provided on top of backbone-es6. However, the larger toolchain should be applicable to any web app framework that can leverage JSPM / SystemJS. 

For native mobile apps TyphonJS provides a pipeline for container based deployment of server / database backends for cloud hosted solutions primarily Parse, Meteor and SocketStream. 

TyphonJS is a multi-organization / repo effort being open sourced under the MPLv2.0 license. A multi org / repo toolchain is currently in development to support TyphonJS and beyond. This approach allows various modules / components of TyphonJS to be mixed and matched more easily. In many ways TyphonJS provides the glue between various important open source development / deployment tooling along with providing additional first party components. All Javascript source code is fully documented and is modern ES6 written in a standard idiomatic style. Please bear with us while the tooling and various framework integrations are completed. Full documentation and testing resources are already provided in most repos and a universal automated documentation repo / web site will be available soon. ETA of an official public launch with tutorials and web site is Q3 '16. 

Below is an overview of all of the TyphonJS organizations / repos as of April 16th 2016. 

----------------

typhonjs](https://github.com/typhonjs) - Provides common repos for TyphonJS

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

[typhonjs-demos-deploy-electron](https://github.com/typhonjs-demos-deploy-electron) - Creates desktop apps using Electron from typhonjs-demos

   - [electron-backbone-es6-localstorage-todos](https://github.com/typhonjs-demos-deploy-electron/electron-backbone-es6-localstorage-todos) - Creates a desktop app  from backbone-es6-localstorage-todos using Electron.
   - [electron-backbone-parse-es6-todos-improved](https://github.com/typhonjs-demos-deploy-electron/electron-backbone-parse-es6-todos-improved) - Creates a desktop app from backbone-parse-es6-todos-improved using Electron.

[typhonjs-demos-test](https://github.com/typhonjs-demos-test) - Provides testing repos specific to issues related to TyphonJS.

   - [istanbul-jspm-coverage-example](https://github.com/typhonjs-demos-test/istanbul-jspm-coverage-example) - Provides an example of instrumenting JSPM / SystemJS for code coverage with Istanbul / Mocha.
   - [typhonjs-issues-demos](https://github.com/typhonjs-demos-test/typhonjs-issues-demos) - Provides various demos for issues raised with all TyphonJS repos.

[typhonjs-docs](https://github.com/typhonjs-docs) - Provides all versioned docs, specs, and governance repos. 

   - [typhonjs-core-docs](https://github.com/typhonjs-docs/typhonjs-core-docs) - Provides overview documentation for all TyphonJS orgs / repos.
   - [typhonjs-core-governance](https://github.com/typhonjs-docs/typhonjs-core-governance) - Provides the authoritative documentation regarding TyphonJS governance.
   - [typhonjs-core-specifications](https://github.com/typhonjs-docs/typhonjs-core-specifications) - Provides overview documentation for all TyphonJS orgs / repos.

[typhonjs-meteor-ddp-client](https://github.com/typhonjs-meteor-ddp-client) - Provides a generic client for DDP (Distributed Data Protocol) and plugin mechanism to link to MVC libraries.

   - [backbone-meteor-es6](https://github.com/typhonjs-meteor-ddp-client/backbone-meteor-es6)
   - [typhonjs-core-asteroid](https://github.com/typhonjs-meteor-ddp-client/typhonjs-core-asteroid) - An ES6 fork of Asteroid providing a generic client for Meteor. 
   - [typhonjs-core-asteroid-belt](https://github.com/typhonjs-meteor-ddp-client/typhonjs-core-asteroid-belt) - Wouldn't you like to know.... coming soon... :D
   - [typhonjs-core-asteroid-init](https://github.com/typhonjs-meteor-ddp-client/typhonjs-core-asteroid-init)
   - [typhonjs-core-socket-ddp](https://github.com/typhonjs-meteor-ddp-client/typhonjs-core-socket-ddp) - Provides a Javascript DDP client

[typhonjs-node-config](https://github.com/typhonjs-node-config) - Provides utility NPM modules for configuration data.

   - [typhonjs-config-eslint](https://github.com/typhonjs-node-config/typhonjs-config-eslint) - Provides shared ESLint configs for TyphonJS repos.

[typhonjs-node-esdoc](https://github.com/typhonjs-node-esdoc) - Provides NPM modules for ESDoc plugins.

   - [esdoc-plugin-dependency-graphs](https://github.com/typhonjs-node-esdoc/esdoc-plugin-dependency-graphs) - A plugin for ESDoc that adds interactive D3 powered dependency graphs for source code including linking JSPM / NPM managed code and packages.
   - [esdoc-plugin-enhanced-navigation](https://github.com/typhonjs-node-esdoc/esdoc-plugin-enhanced-navigation) - Replaces the standard ESDoc left hand source navigation with an enhanced version. 
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
   - [typhonjs-npm-scripts-test-mocha](https://github.com/typhonjs-node-npm-scripts/typhonjs-npm-scripts-test-mocha) - Provides NPM scripts for testing projects using Istanbul & Mocha for all TyphonJS NPM modules and beyond.

[typhonjs-node-scm](https://github.com/typhonjs-node-scm) - Provides utility NPM modules for interfacing with source code management systems.

   - [typhonjs-github-inspect-orgs](https://github.com/typhonjs-node-scm/typhonjs-github-inspect-orgs) - A NPM module providing compound GitHub queries spanning multiple organizations / users for many-repo projects such as TyphonJS.
   - [typhonjs-github-inspect-orgs-transform](https://github.com/typhonjs-node-scm/typhonjs-github-inspect-orgs-transform) - Provides a NPM module that transforms data from typhonjs-github-inspect-orgs to normalized HTML, markdown, JSON or text.

[typhonjs-react](https://github.com/typhonjs-react) - So this is your sandbox React. Bring your best and let's see what you got. 

[typhonjs-react-native](https://github.com/typhonjs-react-native) - Forthcoming support for React Native (IE meteor / DDP support).

[typhonjs-socketstream-client](https://github.com/typhonjs-socketstream-client) - Provides a generic client for SocketStream and plugin mechanism to link to MVC libraries.

[typhonjs-utils](https://github.com/typhonjs-utils) - Provides miscellaneous utility repos.

   - [intellij-plugin-jspm](https://github.com/typhonjs-utils/intellij-plugin-jspm) - Provides JSPM reference and path completion plugin for WebStorm, PHPStorm and other Idea family IDE supporting Javascript.

[typhonjs-zenhub](https://github.com/typhonjs-zenhub) - Provides a common location for all ZenHub projects tracking all repos from each major TyphonJS org category. 

   - [zenhub-typhonjs](https://github.com/typhonjs-zenhub/zenhub-typhonjs) - Provides a ZenHub overview of all TyphonJS orgs / repos.
