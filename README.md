# api documentation for  [vue-cli (v2.8.1)](https://github.com/vuejs/vue-cli#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-vue-cli.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-vue-cli) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-vue-cli.svg)](https://travis-ci.org/npmdoc/node-npmdoc-vue-cli)
#### A simple CLI for scaffolding Vue.js projects.

[![NPM](https://nodei.co/npm/vue-cli.png?downloads=true)](https://www.npmjs.com/package/vue-cli)

[![apidoc](https://npmdoc.github.io/node-npmdoc-vue-cli/build/screenCapture.buildNpmdoc.browser._2Fhome_2Ftravis_2Fbuild_2Fnpmdoc_2Fnode-npmdoc-vue-cli_2Ftmp_2Fbuild_2Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-vue-cli/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-vue-cli/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-vue-cli/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Evan You"
    },
    "bin": {
        "vue": "bin/vue",
        "vue-init": "bin/vue-init",
        "vue-list": "bin/vue-list",
        "vue-build": "bin/vue-build"
    },
    "bugs": {
        "url": "https://github.com/vuejs/vue-cli/issues"
    },
    "dependencies": {
        "async": "^2.0.0-rc.2",
        "autoprefixer": "^6.6.1",
        "babel-core": "^6.21.0",
        "babel-loader": "^6.2.10",
        "babel-preset-vue-app": "^0.4.0",
        "chalk": "^1.1.1",
        "commander": "^2.9.0",
        "connect-history-api-fallback": "^1.3.0",
        "consolidate": "^0.14.0",
        "css-loader": "^0.26.1",
        "download-git-repo": "^0.2.1",
        "express": "^4.14.0",
        "extract-text-webpack-plugin": "2.0.0-beta.5",
        "file-loader": "^0.9.0",
        "friendly-errors-webpack-plugin": "^1.1.2",
        "handlebars": "^4.0.5",
        "html-webpack-plugin": "^2.26.0",
        "http-proxy-middleware": "^0.17.3",
        "inquirer": "^0.12.0",
        "installed-by-yarn-globally": "^0.1.1",
        "metalsmith": "^2.1.0",
        "minimatch": "^3.0.0",
        "multimatch": "^2.1.0",
        "opn": "^4.0.2",
        "ora": "^0.2.1",
        "post-compile-webpack-plugin": "^0.1.0",
        "postcss-loader": "^1.2.1",
        "read-metadata": "^1.0.0",
        "request": "^2.67.0",
        "rimraf": "^2.5.0",
        "semver": "^5.1.0",
        "tildify": "^1.2.0",
        "url-loader": "^0.5.7",
        "user-home": "^2.0.0",
        "validate-npm-package-name": "^2.2.2",
        "vue": "^2.1.10",
        "vue-loader": "^10.0.2",
        "vue-template-compiler": "^2.1.10",
        "webpack": "^2.2.0",
        "webpack-dev-middleware": "^1.9.0",
        "webpack-hot-middleware": "^2.15.0",
        "webpack-merge": "^2.3.1"
    },
    "description": "A simple CLI for scaffolding Vue.js projects.",
    "devDependencies": {
        "chai": "^3.5.0",
        "cross-env": "^1.0.7",
        "eslint": "^2.7.0",
        "eslint-config-standard": "^5.1.0",
        "eslint-plugin-promise": "^1.1.0",
        "eslint-plugin-standard": "^1.3.2",
        "execa": "^0.5.0",
        "mocha": "^2.4.5"
    },
    "directories": {},
    "dist": {
        "shasum": "1f11147346c618a943580a6584b9b7cd55a1bd02",
        "tarball": "https://registry.npmjs.org/vue-cli/-/vue-cli-2.8.1.tgz"
    },
    "engines": {
        "node": ">=4.0.0"
    },
    "gitHead": "c75cb4643de206eea3cd66b62753d98c07500302",
    "homepage": "https://github.com/vuejs/vue-cli#readme",
    "keywords": [
        "vue",
        "cli",
        "spa"
    ],
    "license": "MIT",
    "main": "lib/index.js",
    "maintainers": [
        {
            "name": "yyx990803",
            "email": "yyx990803@gmail.com"
        }
    ],
    "name": "vue-cli",
    "optionalDependencies": {},
    "preferGlobal": true,
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/vuejs/vue-cli.git"
    },
    "scripts": {
        "e2e": "rimraf test/e2e/mock-template-build && cross-env BABEL_ENV=development mocha test/e2e/test.js --slow 1000 --compilers js:babel-core/register",
        "e2e:build": "cross-env BABEL_ENV=development mocha test/e2e/test-build.js --timeout 60000 --compilers js:babel-core/register",
        "lint": "eslint test/e2e/test*.js lib bin/* --env mocha",
        "test": "npm run lint && npm run e2e && npm run e2e:build"
    },
    "version": "2.8.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module vue-cli](#apidoc.module.vue-cli)
1.  object <span class="apidocSignatureSpan">vue-cli.</span>loaders
1.  object <span class="apidocSignatureSpan">vue-cli.</span>logger
1.  object <span class="apidocSignatureSpan">vue-cli.</span>warnings

#### [module vue-cli.loaders](#apidoc.module.vue-cli.loaders)
1.  [function <span class="apidocSignatureSpan">vue-cli.loaders.</span>cssLoaders (options)](#apidoc.element.vue-cli.loaders.cssLoaders)
1.  [function <span class="apidocSignatureSpan">vue-cli.loaders.</span>styleLoaders (options)](#apidoc.element.vue-cli.loaders.styleLoaders)

#### [module vue-cli.logger](#apidoc.module.vue-cli.logger)
1.  [function <span class="apidocSignatureSpan">vue-cli.logger.</span>fatal (message)](#apidoc.element.vue-cli.logger.fatal)
1.  [function <span class="apidocSignatureSpan">vue-cli.logger.</span>log ()](#apidoc.element.vue-cli.logger.log)
1.  [function <span class="apidocSignatureSpan">vue-cli.logger.</span>success ()](#apidoc.element.vue-cli.logger.success)

#### [module vue-cli.warnings](#apidoc.module.vue-cli.warnings)
1.  [function <span class="apidocSignatureSpan">vue-cli.warnings.</span>v2BranchIsNowDefault (template, name)](#apidoc.element.vue-cli.warnings.v2BranchIsNowDefault)
1.  [function <span class="apidocSignatureSpan">vue-cli.warnings.</span>v2SuffixTemplatesDeprecated (template, name)](#apidoc.element.vue-cli.warnings.v2SuffixTemplatesDeprecated)



# <a name="apidoc.module.vue-cli"></a>[module vue-cli](#apidoc.module.vue-cli)



# <a name="apidoc.module.vue-cli.loaders"></a>[module vue-cli.loaders](#apidoc.module.vue-cli.loaders)

#### <a name="apidoc.element.vue-cli.loaders.cssLoaders"></a>[function <span class="apidocSignatureSpan">vue-cli.loaders.</span>cssLoaders (options)](#apidoc.element.vue-cli.loaders.cssLoaders)
- description and source-code
```javascript
cssLoaders = function (options) {
  options = options || {}
  // generate loader string to be used with extract text plugin
  function generateLoaders (loaders) {
    var sourceLoader = loaders.map(function (loader) {
      var extraParamChar
      if (/\?/.test(loader)) {
        loader = loader.replace(/\?/, '-loader?')
        extraParamChar = '&'
      } else {
        loader = loader + '-loader'
        extraParamChar = '?'
      }
      return loader + (options.sourceMap ? extraParamChar + 'sourceMap' : '')
    }).join('!')

    // Extract CSS when that option is specified
    // (which is the case during production build)
    if (options.extract) {
      return ExtractTextPlugin.extract({
        loader: sourceLoader,
        fallbackLoader: 'vue-style-loader'
      })
    } else {
      return ['vue-style-loader', sourceLoader].join('!')
    }
  }

  // http://vuejs.github.io/vue-loader/en/configurations/extract-css.html
  return {
    css: generateLoaders(['css?-autoprefixer', 'postcss']),
    less: generateLoaders(['css?-autoprefixer', 'postcss', 'less']),
    sass: generateLoaders(['css?-autoprefixer', 'postcss', 'sass?indentedSyntax']),
    scss: generateLoaders(['css?-autoprefixer', 'postcss', 'sass']),
    stylus: generateLoaders(['css?-autoprefixer', 'postcss', 'stylus']),
    styl: generateLoaders(['css?-autoprefixer', 'postcss', 'stylus'])
  }
}
```
- example usage
```shell
...
  styl: generateLoaders(['css?-autoprefixer', 'postcss', 'stylus'])
}
}

// Generate loaders for standalone style files (outside of .vue)
exports.styleLoaders = function (options) {
var output = []
var loaders = exports.cssLoaders(options)
for (var extension in loaders) {
  var loader = loaders[extension]
  output.push({
    test: new RegExp('\\.' + extension + '$'),
    loader: loader
  })
}
...
```

#### <a name="apidoc.element.vue-cli.loaders.styleLoaders"></a>[function <span class="apidocSignatureSpan">vue-cli.loaders.</span>styleLoaders (options)](#apidoc.element.vue-cli.loaders.styleLoaders)
- description and source-code
```javascript
styleLoaders = function (options) {
  var output = []
  var loaders = exports.cssLoaders(options)
  for (var extension in loaders) {
    var loader = loaders[extension]
    output.push({
      test: new RegExp('\\.' + extension + '$'),
      loader: loader
    })
  }
  return output
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vue-cli.logger"></a>[module vue-cli.logger](#apidoc.module.vue-cli.logger)

#### <a name="apidoc.element.vue-cli.logger.fatal"></a>[function <span class="apidocSignatureSpan">vue-cli.logger.</span>fatal (message)](#apidoc.element.vue-cli.logger.fatal)
- description and source-code
```javascript
fatal = function (message) {
  if (message instanceof Error) message = message.message.trim()
  var msg = format.apply(format, arguments)
  console.error(chalk.red(prefix), sep, msg)
  process.exit(1)
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue-cli.logger.log"></a>[function <span class="apidocSignatureSpan">vue-cli.logger.</span>log ()](#apidoc.element.vue-cli.logger.log)
- description and source-code
```javascript
log = function () {
  var msg = format.apply(format, arguments)
  console.log(chalk.white(prefix), sep, msg)
}
```
- example usage
```shell
...
var semver = require('semver')
var chalk = require('chalk')
var packageConfig = require('../package.json')

module.exports = function (done) {
// Ensure minimum supported node version is used
if (!semver.satisfies(process.version, packageConfig.engines.node)) {
  return console.log(chalk.red(
    '  You must upgrade node to >=' + packageConfig.engines.node + '.x to use vue-cli'
  ))
}

request({
  url: 'https://registry.npmjs.org/vue-cli',
  timeout: 1000
...
```

#### <a name="apidoc.element.vue-cli.logger.success"></a>[function <span class="apidocSignatureSpan">vue-cli.logger.</span>success ()](#apidoc.element.vue-cli.logger.success)
- description and source-code
```javascript
success = function () {
  var msg = format.apply(format, arguments)
  console.log(chalk.white(prefix), sep, msg)
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.vue-cli.warnings"></a>[module vue-cli.warnings](#apidoc.module.vue-cli.warnings)

#### <a name="apidoc.element.vue-cli.warnings.v2BranchIsNowDefault"></a>[function <span class="apidocSignatureSpan">vue-cli.warnings.</span>v2BranchIsNowDefault (template, name)](#apidoc.element.vue-cli.warnings.v2BranchIsNowDefault)
- description and source-code
```javascript
v2BranchIsNowDefault = function (template, name) {
  var vue1InitCommand = 'vue init ' + template + '#1.0' + ' ' + name

  console.log(chalk.green('  This will install Vue 2.x version of the template.'))
  console.log()
  console.log(chalk.yellow('  For Vue 1.x use: ') + chalk.green(vue1InitCommand))
  console.log()
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.vue-cli.warnings.v2SuffixTemplatesDeprecated"></a>[function <span class="apidocSignatureSpan">vue-cli.warnings.</span>v2SuffixTemplatesDeprecated (template, name)](#apidoc.element.vue-cli.warnings.v2SuffixTemplatesDeprecated)
- description and source-code
```javascript
v2SuffixTemplatesDeprecated = function (template, name) {
  var initCommand = 'vue init ' + template.replace('-2.0', '') + ' ' + name

  console.log(chalk.red('  This template is deprecated, as the original template now uses Vue 2.0 by default.'))
  console.log()
  console.log(chalk.yellow('  Please use this command instead: ') + chalk.green(initCommand))
  console.log()
}
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
