# api documentation for  [react-select (v0.9.1)](https://github.com/JedWatson/react-select#readme)  [![npm package](https://img.shields.io/npm/v/npmdoc-react-select.svg?style=flat-square)](https://www.npmjs.org/package/npmdoc-react-select) [![travis-ci.org build-status](https://api.travis-ci.org/npmdoc/node-npmdoc-react-select.svg)](https://travis-ci.org/npmdoc/node-npmdoc-react-select)
#### A Select control built with and for ReactJS

[![NPM](https://nodei.co/npm/react-select.png?downloads=true)](https://www.npmjs.com/package/react-select)

[![apidoc](https://npmdoc.github.io/node-npmdoc-react-select/build/screenCapture.buildNpmdoc.browser.%252Fhome%252Ftravis%252Fbuild%252Fnpmdoc%252Fnode-npmdoc-react-select%252Ftmp%252Fbuild%252Fapidoc.html.png)](https://npmdoc.github.io/node-npmdoc-react-select/build/apidoc.html)

![npmPackageListing](https://npmdoc.github.io/node-npmdoc-react-select/build/screenCapture.npmPackageListing.svg)

![npmPackageDependencyTree](https://npmdoc.github.io/node-npmdoc-react-select/build/screenCapture.npmPackageDependencyTree.svg)



# package.json

```json

{
    "author": {
        "name": "Jed Watson"
    },
    "browserify-shim": {
        "classnames": "global:classNames",
        "react": "global:React",
        "react-input-autosize": "global:AutosizeInput"
    },
    "bugs": {
        "url": "https://github.com/JedWatson/react-select/issues"
    },
    "dependencies": {
        "classnames": "^2.2.0",
        "react-input-autosize": "^0.6.2"
    },
    "description": "A Select control built with and for ReactJS",
    "devDependencies": {
        "babel": "^5.8.23",
        "babel-eslint": "^4.1.3",
        "chai": "^3.4.0",
        "coveralls": "^2.11.4",
        "eslint": "^1.8.0",
        "eslint-plugin-react": "^3.6.3",
        "gulp": "^3.9.0",
        "istanbul": "^0.4.0",
        "jsdom": "^7.0.2",
        "mocha": "^2.3.3",
        "react": "^0.14.1",
        "react-addons-test-utils": "^0.14.1",
        "react-component-gulp-tasks": "^0.7.7",
        "react-dom": "^0.14.1",
        "react-gravatar": "^2.2.2",
        "sinon": "^1.17.2",
        "unexpected": "^10.0.2",
        "unexpected-dom": "^3.0.2",
        "unexpected-sinon": "^8.0.0"
    },
    "directories": {},
    "dist": {
        "shasum": "e322a2d0a06396a48206b0553df5ec47d16083ba",
        "tarball": "https://registry.npmjs.org/react-select/-/react-select-0.9.1.tgz"
    },
    "gitHead": "d8fe544f32dc28e1f72592671f7c70bddae3258a",
    "homepage": "https://github.com/JedWatson/react-select#readme",
    "keywords": [
        "combobox",
        "form",
        "input",
        "multiselect",
        "react",
        "react-component",
        "select",
        "ui"
    ],
    "license": "MIT",
    "main": "lib/Select.js",
    "maintainers": [
        {
            "name": "jedwatson",
            "email": "jed.watson@me.com"
        }
    ],
    "name": "react-select",
    "optionalDependencies": {},
    "peerDependencies": {
        "react": "^0.14.1",
        "react-dom": "^0.14.1"
    },
    "readme": "ERROR: No README data found!",
    "repository": {
        "type": "git",
        "url": "git+https://github.com/JedWatson/react-select.git"
    },
    "scripts": {
        "build": "gulp clean && NODE_ENV=production gulp build",
        "bump": "gulp bump",
        "bump:major": "gulp bump:major",
        "bump:minor": "gulp bump:minor",
        "cover": "istanbul cover _mocha -- -u exports --compilers js:babel/register -R spec",
        "coveralls": "NODE_ENV=test istanbul cover _mocha --report lcovonly -- -u exports --compilers js:babel/register -R spec && cat coverage/lcov.info | coveralls",
        "examples": "gulp dev:server",
        "lint": "eslint .",
        "publish:examples": "NODE_ENV=production gulp publish:examples",
        "release": "NODE_ENV=production gulp release",
        "start": "gulp dev",
        "test": "mocha --compilers js:babel/register",
        "watch": "gulp watch:lib"
    },
    "style": "dist/default.css",
    "version": "0.9.1"
}
```



# <a name="apidoc.tableOfContents"></a>[table of contents](#apidoc.tableOfContents)

#### [module react-select](#apidoc.module.react-select)
1.  [function <span class="apidocSignatureSpan">react-select.</span>defaultProps.optionComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.optionComponent)
1.  [function <span class="apidocSignatureSpan">react-select.</span>defaultProps.singleValueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.singleValueComponent)
1.  [function <span class="apidocSignatureSpan">react-select.</span>defaultProps.valueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.valueComponent)
1.  [function <span class="apidocSignatureSpan">react-select.</span>getDefaultProps ()](#apidoc.element.react-select.getDefaultProps)
1.  [function <span class="apidocSignatureSpan">react-select.</span>propTypes.addLabelText ()](#apidoc.element.react-select.propTypes.addLabelText)
1.  [function <span class="apidocSignatureSpan">react-select.</span>propTypes.allowCreate ()](#apidoc.element.react-select.propTypes.allowCreate)
1.  [function <span class="apidocSignatureSpan">react-select.</span>propTypes.asyncOptions ()](#apidoc.element.react-select.propTypes.asyncOptions)
1.  [function <span class="apidocSignatureSpan">react-select.</span>propTypes.inputProps ()](#apidoc.element.react-select.propTypes.inputProps)
1.  [function <span class="apidocSignatureSpan">react-select.</span>propTypes.options ()](#apidoc.element.react-select.propTypes.options)
1.  [function <span class="apidocSignatureSpan">react-select.</span>propTypes.value ()](#apidoc.element.react-select.propTypes.value)
1.  object <span class="apidocSignatureSpan">react-select.</span>defaultProps
1.  object <span class="apidocSignatureSpan">react-select.</span>defaultProps.optionComponent.prototype
1.  object <span class="apidocSignatureSpan">react-select.</span>defaultProps.optionComponent.prototype.__reactAutoBindMap
1.  object <span class="apidocSignatureSpan">react-select.</span>defaultProps.singleValueComponent.prototype
1.  object <span class="apidocSignatureSpan">react-select.</span>defaultProps.singleValueComponent.prototype.__reactAutoBindMap
1.  object <span class="apidocSignatureSpan">react-select.</span>defaultProps.valueComponent.prototype
1.  object <span class="apidocSignatureSpan">react-select.</span>defaultProps.valueComponent.prototype.__reactAutoBindMap
1.  object <span class="apidocSignatureSpan">react-select.</span>nodeListType
1.  object <span class="apidocSignatureSpan">react-select.</span>propTypes
1.  string <span class="apidocSignatureSpan">react-select.</span>displayName

#### [module react-select.defaultProps](#apidoc.module.react-select.defaultProps)
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>allowCreate
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>autoload
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>backspaceRemoves
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>cacheAsyncResults
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>clearable
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>disabled
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>ignoreCase
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>isLoading
1.  boolean <span class="apidocSignatureSpan">react-select.defaultProps.</span>searchable
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.</span>optionComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.optionComponent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.</span>singleValueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.singleValueComponent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.</span>valueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.valueComponent)
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.</span>inputProps
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>addLabelText
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>clearAllText
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>clearValueText
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>delimiter
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>labelKey
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>matchPos
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>matchProp
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>noResultsText
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>placeholder
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>searchPromptText
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>searchingText
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.</span>valueKey

#### [module react-select.defaultProps.optionComponent](#apidoc.module.react-select.defaultProps.optionComponent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.</span>optionComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.optionComponent.optionComponent)
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.</span>propTypes
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.</span>displayName

#### [module react-select.defaultProps.optionComponent.prototype](#apidoc.module.react-select.defaultProps.optionComponent.prototype)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>blockEvent (event)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.blockEvent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>constructor (props, context, updater)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.optionComponent.prototype.getDOMNode)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>handleMouseDown (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseDown)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>handleMouseEnter (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseEnter)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>handleMouseLeave (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseLeave)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>render ()](#apidoc.element.react-select.defaultProps.optionComponent.prototype.render)
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>__reactAutoBindMap
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>childContextTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>componentDidMount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>componentDidUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>componentWillMount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>componentWillReceiveProps
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>componentWillUnmount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>componentWillUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>contextTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>getChildContext
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>getDefaultProps
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>getInitialState
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>mixins
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>propTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>shouldComponentUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>statics
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>updateComponent

#### [module react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap](#apidoc.module.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>blockEvent (event)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.blockEvent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.getDOMNode)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>handleMouseDown (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseDown)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>handleMouseEnter (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseEnter)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>handleMouseLeave (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseLeave)

#### [module react-select.defaultProps.singleValueComponent](#apidoc.module.react-select.defaultProps.singleValueComponent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.</span>singleValueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.singleValueComponent.singleValueComponent)
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.</span>propTypes
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.</span>displayName

#### [module react-select.defaultProps.singleValueComponent.prototype](#apidoc.module.react-select.defaultProps.singleValueComponent.prototype)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>constructor (props, context, updater)](#apidoc.element.react-select.defaultProps.singleValueComponent.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.singleValueComponent.prototype.getDOMNode)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>render ()](#apidoc.element.react-select.defaultProps.singleValueComponent.prototype.render)
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>__reactAutoBindMap
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>childContextTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>componentDidMount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>componentDidUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>componentWillMount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>componentWillReceiveProps
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>componentWillUnmount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>componentWillUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>contextTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>getChildContext
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>getDefaultProps
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>getInitialState
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>mixins
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>propTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>shouldComponentUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>statics
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>updateComponent

#### [module react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap](#apidoc.module.react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap.getDOMNode)

#### [module react-select.defaultProps.valueComponent](#apidoc.module.react-select.defaultProps.valueComponent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.</span>valueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.valueComponent.valueComponent)
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.</span>propTypes
1.  string <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.</span>displayName

#### [module react-select.defaultProps.valueComponent.prototype](#apidoc.module.react-select.defaultProps.valueComponent.prototype)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>blockEvent (event)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.blockEvent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>constructor (props, context, updater)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.constructor)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.valueComponent.prototype.getDOMNode)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>handleOnRemove (event)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.handleOnRemove)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>render ()](#apidoc.element.react-select.defaultProps.valueComponent.prototype.render)
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>__reactAutoBindMap
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>childContextTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>componentDidMount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>componentDidUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>componentWillMount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>componentWillReceiveProps
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>componentWillUnmount
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>componentWillUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>contextTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>getChildContext
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>getDefaultProps
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>getInitialState
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>mixins
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>propTypes
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>shouldComponentUpdate
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>statics
1.  object <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>updateComponent

#### [module react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap](#apidoc.module.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.</span>blockEvent (event)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.blockEvent)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.getDOMNode)
1.  [function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.</span>handleOnRemove (event)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.handleOnRemove)

#### [module react-select.nodeListType](#apidoc.module.react-select.nodeListType)
1.  [function <span class="apidocSignatureSpan">react-select.nodeListType.</span>installInto (expect)](#apidoc.element.react-select.nodeListType.installInto)
1.  string <span class="apidocSignatureSpan">react-select.nodeListType.</span>name

#### [module react-select.propTypes](#apidoc.module.react-select.propTypes)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>addLabelText ()](#apidoc.element.react-select.propTypes.addLabelText)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>allowCreate ()](#apidoc.element.react-select.propTypes.allowCreate)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>asyncOptions ()](#apidoc.element.react-select.propTypes.asyncOptions)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>autoload ()](#apidoc.element.react-select.propTypes.autoload)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>backspaceRemoves ()](#apidoc.element.react-select.propTypes.backspaceRemoves)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>cacheAsyncResults ()](#apidoc.element.react-select.propTypes.cacheAsyncResults)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>className ()](#apidoc.element.react-select.propTypes.className)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>clearAllText ()](#apidoc.element.react-select.propTypes.clearAllText)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>clearValueText ()](#apidoc.element.react-select.propTypes.clearValueText)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>clearable ()](#apidoc.element.react-select.propTypes.clearable)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>delimiter ()](#apidoc.element.react-select.propTypes.delimiter)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>disabled ()](#apidoc.element.react-select.propTypes.disabled)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>filterOption ()](#apidoc.element.react-select.propTypes.filterOption)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>filterOptions ()](#apidoc.element.react-select.propTypes.filterOptions)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>ignoreCase ()](#apidoc.element.react-select.propTypes.ignoreCase)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>inputProps ()](#apidoc.element.react-select.propTypes.inputProps)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>isLoading ()](#apidoc.element.react-select.propTypes.isLoading)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>labelKey ()](#apidoc.element.react-select.propTypes.labelKey)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>matchPos ()](#apidoc.element.react-select.propTypes.matchPos)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>matchProp ()](#apidoc.element.react-select.propTypes.matchProp)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>multi ()](#apidoc.element.react-select.propTypes.multi)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>name ()](#apidoc.element.react-select.propTypes.name)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>newOptionCreator ()](#apidoc.element.react-select.propTypes.newOptionCreator)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>noResultsText ()](#apidoc.element.react-select.propTypes.noResultsText)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>onBlur ()](#apidoc.element.react-select.propTypes.onBlur)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>onChange ()](#apidoc.element.react-select.propTypes.onChange)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>onFocus ()](#apidoc.element.react-select.propTypes.onFocus)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>onInputChange ()](#apidoc.element.react-select.propTypes.onInputChange)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>onOptionLabelClick ()](#apidoc.element.react-select.propTypes.onOptionLabelClick)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>optionComponent ()](#apidoc.element.react-select.propTypes.optionComponent)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>optionRenderer ()](#apidoc.element.react-select.propTypes.optionRenderer)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>options ()](#apidoc.element.react-select.propTypes.options)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>placeholder ()](#apidoc.element.react-select.propTypes.placeholder)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>searchPromptText ()](#apidoc.element.react-select.propTypes.searchPromptText)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>searchable ()](#apidoc.element.react-select.propTypes.searchable)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>searchingText ()](#apidoc.element.react-select.propTypes.searchingText)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>singleValueComponent ()](#apidoc.element.react-select.propTypes.singleValueComponent)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>value ()](#apidoc.element.react-select.propTypes.value)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>valueComponent ()](#apidoc.element.react-select.propTypes.valueComponent)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>valueKey ()](#apidoc.element.react-select.propTypes.valueKey)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>valueRenderer ()](#apidoc.element.react-select.propTypes.valueRenderer)

#### [module react-select.propTypes.addLabelText](#apidoc.module.react-select.propTypes.addLabelText)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>addLabelText ()](#apidoc.element.react-select.propTypes.addLabelText.addLabelText)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.addLabelText.</span>isRequired ()](#apidoc.element.react-select.propTypes.addLabelText.isRequired)

#### [module react-select.propTypes.allowCreate](#apidoc.module.react-select.propTypes.allowCreate)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>allowCreate ()](#apidoc.element.react-select.propTypes.allowCreate.allowCreate)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.allowCreate.</span>isRequired ()](#apidoc.element.react-select.propTypes.allowCreate.isRequired)

#### [module react-select.propTypes.asyncOptions](#apidoc.module.react-select.propTypes.asyncOptions)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>asyncOptions ()](#apidoc.element.react-select.propTypes.asyncOptions.asyncOptions)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.asyncOptions.</span>isRequired ()](#apidoc.element.react-select.propTypes.asyncOptions.isRequired)

#### [module react-select.propTypes.inputProps](#apidoc.module.react-select.propTypes.inputProps)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>inputProps ()](#apidoc.element.react-select.propTypes.inputProps.inputProps)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.inputProps.</span>isRequired ()](#apidoc.element.react-select.propTypes.inputProps.isRequired)

#### [module react-select.propTypes.options](#apidoc.module.react-select.propTypes.options)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>options ()](#apidoc.element.react-select.propTypes.options.options)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.options.</span>isRequired ()](#apidoc.element.react-select.propTypes.options.isRequired)

#### [module react-select.propTypes.value](#apidoc.module.react-select.propTypes.value)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.</span>value ()](#apidoc.element.react-select.propTypes.value.value)
1.  [function <span class="apidocSignatureSpan">react-select.propTypes.value.</span>isRequired ()](#apidoc.element.react-select.propTypes.value.isRequired)



# <a name="apidoc.module.react-select"></a>[module react-select](#apidoc.module.react-select)

#### <a name="apidoc.element.react-select.defaultProps.optionComponent"></a>[function <span class="apidocSignatureSpan">react-select.</span>defaultProps.optionComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.optionComponent)
- description and source-code
```javascript
defaultProps.optionComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.singleValueComponent"></a>[function <span class="apidocSignatureSpan">react-select.</span>defaultProps.singleValueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.singleValueComponent)
- description and source-code
```javascript
defaultProps.singleValueComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.valueComponent"></a>[function <span class="apidocSignatureSpan">react-select.</span>defaultProps.valueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.valueComponent)
- description and source-code
```javascript
defaultProps.valueComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.getDefaultProps"></a>[function <span class="apidocSignatureSpan">react-select.</span>getDefaultProps ()](#apidoc.element.react-select.getDefaultProps)
- description and source-code
```javascript
function getDefaultProps() {
		return {
			addLabelText: 'Add "{label}"?',
			allowCreate: false,
			asyncOptions: undefined,
			autoload: true,
			backspaceRemoves: true,
			cacheAsyncResults: true,
			className: undefined,
			clearAllText: 'Clear all',
			clearValueText: 'Clear value',
			clearable: true,
			delimiter: ',',
			disabled: false,
			ignoreCase: true,
			inputProps: {},
			isLoading: false,
			labelKey: 'label',
			matchPos: 'any',
			matchProp: 'any',
			name: undefined,
			newOptionCreator: undefined,
			noResultsText: 'No results found',
			onChange: undefined,
			onInputChange: undefined,
			onOptionLabelClick: undefined,
			optionComponent: Option,
			options: undefined,
			placeholder: 'Select...',
			searchable: true,
			searchingText: 'Searching...',
			searchPromptText: 'Type to search',
			singleValueComponent: SingleValue,
			value: undefined,
			valueComponent: Value,
			valueKey: 'value'
		};
	}
```
- example usage
```shell
...
  mixSpecIntoComponent.bind(null, Constructor)
);

mixSpecIntoComponent(Constructor, spec);

// Initialize the defaultProps property after all mixins have been merged
if (Constructor.getDefaultProps) {
  Constructor.defaultProps = Constructor.getDefaultProps();
}

if ("production" !== process.env.NODE_ENV) {
  // This is a tag to indicate that the use of these method names is ok,
  // since it's used with createClass. If it's not, then it's likely a
  // mistake so we'll warn you to use the static property, property
  // initializer or constructor respectively.
...
```

#### <a name="apidoc.element.react-select.propTypes.addLabelText"></a>[function <span class="apidocSignatureSpan">react-select.</span>propTypes.addLabelText ()](#apidoc.element.react-select.propTypes.addLabelText)
- description and source-code
```javascript
propTypes.addLabelText = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.allowCreate"></a>[function <span class="apidocSignatureSpan">react-select.</span>propTypes.allowCreate ()](#apidoc.element.react-select.propTypes.allowCreate)
- description and source-code
```javascript
propTypes.allowCreate = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.asyncOptions"></a>[function <span class="apidocSignatureSpan">react-select.</span>propTypes.asyncOptions ()](#apidoc.element.react-select.propTypes.asyncOptions)
- description and source-code
```javascript
propTypes.asyncOptions = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.inputProps"></a>[function <span class="apidocSignatureSpan">react-select.</span>propTypes.inputProps ()](#apidoc.element.react-select.propTypes.inputProps)
- description and source-code
```javascript
propTypes.inputProps = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.options"></a>[function <span class="apidocSignatureSpan">react-select.</span>propTypes.options ()](#apidoc.element.react-select.propTypes.options)
- description and source-code
```javascript
propTypes.options = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.value"></a>[function <span class="apidocSignatureSpan">react-select.</span>propTypes.value ()](#apidoc.element.react-select.propTypes.value)
- description and source-code
```javascript
propTypes.value = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.defaultProps"></a>[module react-select.defaultProps](#apidoc.module.react-select.defaultProps)

#### <a name="apidoc.element.react-select.defaultProps.optionComponent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.</span>optionComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.optionComponent)
- description and source-code
```javascript
optionComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.singleValueComponent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.</span>singleValueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.singleValueComponent)
- description and source-code
```javascript
singleValueComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.valueComponent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.</span>valueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.valueComponent)
- description and source-code
```javascript
valueComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.defaultProps.optionComponent"></a>[module react-select.defaultProps.optionComponent](#apidoc.module.react-select.defaultProps.optionComponent)

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.optionComponent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.</span>optionComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.optionComponent.optionComponent)
- description and source-code
```javascript
optionComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.defaultProps.optionComponent.prototype"></a>[module react-select.defaultProps.optionComponent.prototype](#apidoc.module.react-select.defaultProps.optionComponent.prototype)

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.blockEvent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>blockEvent (event)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.blockEvent)
- description and source-code
```javascript
function blockEvent(event) {
		event.preventDefault();
		if (event.target.tagName !== 'A' || !('href' in event.target)) {
			return;
		}

		if (event.target.target) {
			window.open(event.target.href);
		} else {
			window.location.href = event.target.href;
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.constructor"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>constructor (props, context, updater)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.constructor)
- description and source-code
```javascript
constructor = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.getDOMNode"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.optionComponent.prototype.getDOMNode)
- description and source-code
```javascript
getDOMNode = function () {
  process.env.NODE_ENV !== 'production' ? warning(this.constructor[didWarnKey], '%s.getDOMNode(...) is deprecated. Please use ' + '
ReactDOM.findDOMNode(instance) instead.', ReactInstanceMap.get(this).getName() || this.tagName || 'Unknown') : undefined;
  this.constructor[didWarnKey] = true;
  return findDOMNode(this);
}
```
- example usage
```shell
...
'use strict';

var focusNode = require("./focusNode");

var AutoFocusMixin = {
  componentDidMount: function() {
    if (this.props.autoFocus) {
      focusNode(this.getDOMNode());
    }
  }
};

module.exports = AutoFocusMixin;

},{"./focusNode":120}],3:[function(require,module,exports){
...
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseDown"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>handleMouseDown (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseDown)
- description and source-code
```javascript
function handleMouseDown(e) {
		this.props.mouseDown(this.props.option, e);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseEnter"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>handleMouseEnter (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseEnter)
- description and source-code
```javascript
function handleMouseEnter(e) {
		this.props.mouseEnter(this.props.option, e);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseLeave"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>handleMouseLeave (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.handleMouseLeave)
- description and source-code
```javascript
function handleMouseLeave(e) {
		this.props.mouseLeave(this.props.option, e);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.render"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.</span>render ()](#apidoc.element.react-select.defaultProps.optionComponent.prototype.render)
- description and source-code
```javascript
function render() {
		var option = this.props.option;
		var label = option.create ? this.props.addLabelText.replace('{label}', option.label) : this.props.renderFunc(option);
		var optionClasses = classes(this.props.className, option.className);

		return option.disabled ? React.createElement(
			'div',
			{ className: optionClasses,
				onMouseDown: this.blockEvent,
				onClick: this.blockEvent },
			label
		) : React.createElement(
			'div',
			{ className: optionClasses,
				style: option.style,
				onMouseDown: this.handleMouseDown,
				onMouseEnter: this.handleMouseEnter,
				onMouseLeave: this.handleMouseLeave,
				onClick: this.handleMouseDown,
				title: option.title },
			label
		);
	}
```
- example usage
```shell
...
},

/**
 * @protected
 */
_renderValidatedComponentWithoutOwnerOrContext: function() {
  var inst = this._instance;
  var renderedComponent = inst.render();
  if ("production" !== process.env.NODE_ENV) {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof renderedComponent === 'undefined' &&
        inst.render._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      renderedComponent = null;
...
```



# <a name="apidoc.module.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap"></a>[module react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap](#apidoc.module.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap)

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.blockEvent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>blockEvent (event)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.blockEvent)
- description and source-code
```javascript
function blockEvent(event) {
		event.preventDefault();
		if (event.target.tagName !== 'A' || !('href' in event.target)) {
			return;
		}

		if (event.target.target) {
			window.open(event.target.href);
		} else {
			window.location.href = event.target.href;
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.getDOMNode"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.getDOMNode)
- description and source-code
```javascript
getDOMNode = function () {
  process.env.NODE_ENV !== 'production' ? warning(this.constructor[didWarnKey], '%s.getDOMNode(...) is deprecated. Please use ' + '
ReactDOM.findDOMNode(instance) instead.', ReactInstanceMap.get(this).getName() || this.tagName || 'Unknown') : undefined;
  this.constructor[didWarnKey] = true;
  return findDOMNode(this);
}
```
- example usage
```shell
...
'use strict';

var focusNode = require("./focusNode");

var AutoFocusMixin = {
  componentDidMount: function() {
    if (this.props.autoFocus) {
      focusNode(this.getDOMNode());
    }
  }
};

module.exports = AutoFocusMixin;

},{"./focusNode":120}],3:[function(require,module,exports){
...
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseDown"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>handleMouseDown (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseDown)
- description and source-code
```javascript
function handleMouseDown(e) {
		this.props.mouseDown(this.props.option, e);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseEnter"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>handleMouseEnter (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseEnter)
- description and source-code
```javascript
function handleMouseEnter(e) {
		this.props.mouseEnter(this.props.option, e);
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseLeave"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.</span>handleMouseLeave (e)](#apidoc.element.react-select.defaultProps.optionComponent.prototype.__reactAutoBindMap.handleMouseLeave)
- description and source-code
```javascript
function handleMouseLeave(e) {
		this.props.mouseLeave(this.props.option, e);
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.defaultProps.singleValueComponent"></a>[module react-select.defaultProps.singleValueComponent](#apidoc.module.react-select.defaultProps.singleValueComponent)

#### <a name="apidoc.element.react-select.defaultProps.singleValueComponent.singleValueComponent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.</span>singleValueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.singleValueComponent.singleValueComponent)
- description and source-code
```javascript
singleValueComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.defaultProps.singleValueComponent.prototype"></a>[module react-select.defaultProps.singleValueComponent.prototype](#apidoc.module.react-select.defaultProps.singleValueComponent.prototype)

#### <a name="apidoc.element.react-select.defaultProps.singleValueComponent.prototype.constructor"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>constructor (props, context, updater)](#apidoc.element.react-select.defaultProps.singleValueComponent.prototype.constructor)
- description and source-code
```javascript
constructor = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.singleValueComponent.prototype.getDOMNode"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.singleValueComponent.prototype.getDOMNode)
- description and source-code
```javascript
getDOMNode = function () {
  process.env.NODE_ENV !== 'production' ? warning(this.constructor[didWarnKey], '%s.getDOMNode(...) is deprecated. Please use ' + '
ReactDOM.findDOMNode(instance) instead.', ReactInstanceMap.get(this).getName() || this.tagName || 'Unknown') : undefined;
  this.constructor[didWarnKey] = true;
  return findDOMNode(this);
}
```
- example usage
```shell
...
'use strict';

var focusNode = require("./focusNode");

var AutoFocusMixin = {
  componentDidMount: function() {
    if (this.props.autoFocus) {
      focusNode(this.getDOMNode());
    }
  }
};

module.exports = AutoFocusMixin;

},{"./focusNode":120}],3:[function(require,module,exports){
...
```

#### <a name="apidoc.element.react-select.defaultProps.singleValueComponent.prototype.render"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.</span>render ()](#apidoc.element.react-select.defaultProps.singleValueComponent.prototype.render)
- description and source-code
```javascript
function render() {
		var classNames = classes('Select-placeholder', this.props.value && this.props.value.className);
		return React.createElement(
			'div',
			{
				className: classNames,
				style: this.props.value && this.props.value.style,
				title: this.props.value && this.props.value.title
			},
			this.props.placeholder
		);
	}
```
- example usage
```shell
...
},

/**
 * @protected
 */
_renderValidatedComponentWithoutOwnerOrContext: function() {
  var inst = this._instance;
  var renderedComponent = inst.render();
  if ("production" !== process.env.NODE_ENV) {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof renderedComponent === 'undefined' &&
        inst.render._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      renderedComponent = null;
...
```



# <a name="apidoc.module.react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap"></a>[module react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap](#apidoc.module.react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap)

#### <a name="apidoc.element.react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap.getDOMNode"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.singleValueComponent.prototype.__reactAutoBindMap.getDOMNode)
- description and source-code
```javascript
getDOMNode = function () {
  process.env.NODE_ENV !== 'production' ? warning(this.constructor[didWarnKey], '%s.getDOMNode(...) is deprecated. Please use ' + '
ReactDOM.findDOMNode(instance) instead.', ReactInstanceMap.get(this).getName() || this.tagName || 'Unknown') : undefined;
  this.constructor[didWarnKey] = true;
  return findDOMNode(this);
}
```
- example usage
```shell
...
'use strict';

var focusNode = require("./focusNode");

var AutoFocusMixin = {
  componentDidMount: function() {
    if (this.props.autoFocus) {
      focusNode(this.getDOMNode());
    }
  }
};

module.exports = AutoFocusMixin;

},{"./focusNode":120}],3:[function(require,module,exports){
...
```



# <a name="apidoc.module.react-select.defaultProps.valueComponent"></a>[module react-select.defaultProps.valueComponent](#apidoc.module.react-select.defaultProps.valueComponent)

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.valueComponent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.</span>valueComponent (props, context, updater)](#apidoc.element.react-select.defaultProps.valueComponent.valueComponent)
- description and source-code
```javascript
valueComponent = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.defaultProps.valueComponent.prototype"></a>[module react-select.defaultProps.valueComponent.prototype](#apidoc.module.react-select.defaultProps.valueComponent.prototype)

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.prototype.blockEvent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>blockEvent (event)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.blockEvent)
- description and source-code
```javascript
function blockEvent(event) {
		event.stopPropagation();
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.prototype.constructor"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>constructor (props, context, updater)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.constructor)
- description and source-code
```javascript
constructor = function (props, context, updater) {
  // This constructor is overridden by mocks. The argument is used
  // by mocks to assert on what gets mounted.

  if (process.env.NODE_ENV !== 'production') {
    process.env.NODE_ENV !== 'production' ? warning(this instanceof Constructor, 'Something is calling a React component directly
. Use a factory or ' + 'JSX instead. See: https://fb.me/react-legacyfactory') : undefined;
  }

  // Wire up auto-binding
  if (this.__reactAutoBindMap) {
    bindAutoBindMethods(this);
  }

  this.props = props;
  this.context = context;
  this.refs = emptyObject;
  this.updater = updater || ReactNoopUpdateQueue;

  this.state = null;

  // ReactClasses doesn't have constructors. Instead, they use the
  // getInitialState and componentWillMount methods for initialization.

  var initialState = this.getInitialState ? this.getInitialState() : null;
  if (process.env.NODE_ENV !== 'production') {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof initialState === 'undefined' && this.getInitialState._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      initialState = null;
    }
  }
  !(typeof initialState === 'object' && !Array.isArray(initialState)) ? process.env.NODE_ENV !== 'production' ? invariant(false, '%
s.getInitialState(): must return an object or null', Constructor.displayName || 'ReactCompositeComponent') : invariant(false) :
undefined;

  this.state = initialState;
}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.prototype.getDOMNode"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.valueComponent.prototype.getDOMNode)
- description and source-code
```javascript
getDOMNode = function () {
  process.env.NODE_ENV !== 'production' ? warning(this.constructor[didWarnKey], '%s.getDOMNode(...) is deprecated. Please use ' + '
ReactDOM.findDOMNode(instance) instead.', ReactInstanceMap.get(this).getName() || this.tagName || 'Unknown') : undefined;
  this.constructor[didWarnKey] = true;
  return findDOMNode(this);
}
```
- example usage
```shell
...
'use strict';

var focusNode = require("./focusNode");

var AutoFocusMixin = {
  componentDidMount: function() {
    if (this.props.autoFocus) {
      focusNode(this.getDOMNode());
    }
  }
};

module.exports = AutoFocusMixin;

},{"./focusNode":120}],3:[function(require,module,exports){
...
```

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.prototype.handleOnRemove"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>handleOnRemove (event)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.handleOnRemove)
- description and source-code
```javascript
function handleOnRemove(event) {
		if (!this.props.disabled) {
			this.props.onRemove(event);
		}
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.prototype.render"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.</span>render ()](#apidoc.element.react-select.defaultProps.valueComponent.prototype.render)
- description and source-code
```javascript
function render() {
		var label = this.props.option.label;
		if (this.props.renderer) {
			label = this.props.renderer(this.props.option);
		}

		if (!this.props.onRemove && !this.props.optionLabelClick) {
			return React.createElement(
				'div',
				{
					className: classes('Select-value', this.props.option.className),
					style: this.props.option.style,
					title: this.props.option.title
				},
				label
			);
		}

		if (this.props.optionLabelClick) {
			label = React.createElement(
				'a',
				{ className: classes('Select-item-label__a', this.props.option.className),
					onMouseDown: this.blockEvent,
					onTouchEnd: this.props.onOptionLabelClick,
					onClick: this.props.onOptionLabelClick,
					style: this.props.option.style,
					title: this.props.option.title },
				label
			);
		}

		return React.createElement(
			'div',
			{ className: classes('Select-item', this.props.option.className),
				style: this.props.option.style,
				title: this.props.option.title },
			React.createElement(
				'span',
				{ className: 'Select-item-icon',
					onMouseDown: this.blockEvent,
					onClick: this.handleOnRemove,
					onTouchEnd: this.handleOnRemove },
				'×'
			),
			React.createElement(
				'span',
				{ className: 'Select-item-label' },
				label
			)
		);
	}
```
- example usage
```shell
...
},

/**
 * @protected
 */
_renderValidatedComponentWithoutOwnerOrContext: function() {
  var inst = this._instance;
  var renderedComponent = inst.render();
  if ("production" !== process.env.NODE_ENV) {
    // We allow auto-mocks to proceed as if they're returning null.
    if (typeof renderedComponent === 'undefined' &&
        inst.render._isMockFunction) {
      // This is probably bad practice. Consider warning here and
      // deprecating this convenience.
      renderedComponent = null;
...
```



# <a name="apidoc.module.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap"></a>[module react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap](#apidoc.module.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap)

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.blockEvent"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.</span>blockEvent (event)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.blockEvent)
- description and source-code
```javascript
function blockEvent(event) {
		event.stopPropagation();
	}
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.getDOMNode"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.</span>getDOMNode ()](#apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.getDOMNode)
- description and source-code
```javascript
getDOMNode = function () {
  process.env.NODE_ENV !== 'production' ? warning(this.constructor[didWarnKey], '%s.getDOMNode(...) is deprecated. Please use ' + '
ReactDOM.findDOMNode(instance) instead.', ReactInstanceMap.get(this).getName() || this.tagName || 'Unknown') : undefined;
  this.constructor[didWarnKey] = true;
  return findDOMNode(this);
}
```
- example usage
```shell
...
'use strict';

var focusNode = require("./focusNode");

var AutoFocusMixin = {
  componentDidMount: function() {
    if (this.props.autoFocus) {
      focusNode(this.getDOMNode());
    }
  }
};

module.exports = AutoFocusMixin;

},{"./focusNode":120}],3:[function(require,module,exports){
...
```

#### <a name="apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.handleOnRemove"></a>[function <span class="apidocSignatureSpan">react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.</span>handleOnRemove (event)](#apidoc.element.react-select.defaultProps.valueComponent.prototype.__reactAutoBindMap.handleOnRemove)
- description and source-code
```javascript
function handleOnRemove(event) {
		if (!this.props.disabled) {
			this.props.onRemove(event);
		}
	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.nodeListType"></a>[module react-select.nodeListType](#apidoc.module.react-select.nodeListType)

#### <a name="apidoc.element.react-select.nodeListType.installInto"></a>[function <span class="apidocSignatureSpan">react-select.nodeListType.</span>installInto (expect)](#apidoc.element.react-select.nodeListType.installInto)
- description and source-code
```javascript
installInto = function (expect) {

		expect.addType({
			name: 'NodeList',
			base: 'array-like',
			identify: value => {
				return typeof window !== 'undefined' &&
					typeof window.NodeList === 'function' &&
					value instanceof window.NodeList;
			}
		});

	}
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.propTypes"></a>[module react-select.propTypes](#apidoc.module.react-select.propTypes)

#### <a name="apidoc.element.react-select.propTypes.addLabelText"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>addLabelText ()](#apidoc.element.react-select.propTypes.addLabelText)
- description and source-code
```javascript
addLabelText = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.allowCreate"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>allowCreate ()](#apidoc.element.react-select.propTypes.allowCreate)
- description and source-code
```javascript
allowCreate = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.asyncOptions"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>asyncOptions ()](#apidoc.element.react-select.propTypes.asyncOptions)
- description and source-code
```javascript
asyncOptions = function () { [native code] }
```
- example usage
```shell
...
					this.setState(newState);
					if (callback) callback.call(this, newState);
					return;
				}
			}
		}

		this.props.asyncOptions(input, function (err, data) {
			if (err) throw err;
			if (_this6.props.cacheAsyncResults) {
				_this6._optionsCache[input] = data;
			}
			if (thisRequestId !== _this6._currentRequestId) {
				return;
			}
...
```

#### <a name="apidoc.element.react-select.propTypes.autoload"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>autoload ()](#apidoc.element.react-select.propTypes.autoload)
- description and source-code
```javascript
autoload = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.backspaceRemoves"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>backspaceRemoves ()](#apidoc.element.react-select.propTypes.backspaceRemoves)
- description and source-code
```javascript
backspaceRemoves = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.cacheAsyncResults"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>cacheAsyncResults ()](#apidoc.element.react-select.propTypes.cacheAsyncResults)
- description and source-code
```javascript
cacheAsyncResults = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.className"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>className ()](#apidoc.element.react-select.propTypes.className)
- description and source-code
```javascript
className = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.clearAllText"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>clearAllText ()](#apidoc.element.react-select.propTypes.clearAllText)
- description and source-code
```javascript
clearAllText = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.clearValueText"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>clearValueText ()](#apidoc.element.react-select.propTypes.clearValueText)
- description and source-code
```javascript
clearValueText = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.clearable"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>clearable ()](#apidoc.element.react-select.propTypes.clearable)
- description and source-code
```javascript
clearable = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.delimiter"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>delimiter ()](#apidoc.element.react-select.propTypes.delimiter)
- description and source-code
```javascript
delimiter = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.disabled"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>disabled ()](#apidoc.element.react-select.propTypes.disabled)
- description and source-code
```javascript
disabled = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.filterOption"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>filterOption ()](#apidoc.element.react-select.propTypes.filterOption)
- description and source-code
```javascript
filterOption = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.filterOptions"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>filterOptions ()](#apidoc.element.react-select.propTypes.filterOptions)
- description and source-code
```javascript
filterOptions = function () { [native code] }
```
- example usage
```shell
...
		var _this2 = this;

		var optionsChanged = false;
		if (JSON.stringify(newProps.options) !== JSON.stringify(this.props.options)) {
			optionsChanged = true;
			this.setState({
				options: newProps.options,
				filteredOptions: this.filterOptions(newProps.options)
			});
		}
		if (newProps.value !== this.state.value || newProps.placeholder !== this.props.placeholder || optionsChanged) {
			var setState = function setState(newState) {
				_this2.setState(_this2.getStateFromValue(newProps.value, newState && newState.options || newProps.options, newProps.placeholder
));
			};
			if (this.props.asyncOptions) {
...
```

#### <a name="apidoc.element.react-select.propTypes.ignoreCase"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>ignoreCase ()](#apidoc.element.react-select.propTypes.ignoreCase)
- description and source-code
```javascript
ignoreCase = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.inputProps"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>inputProps ()](#apidoc.element.react-select.propTypes.inputProps)
- description and source-code
```javascript
inputProps = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.isLoading"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>isLoading ()](#apidoc.element.react-select.propTypes.isLoading)
- description and source-code
```javascript
isLoading = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.labelKey"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>labelKey ()](#apidoc.element.react-select.propTypes.labelKey)
- description and source-code
```javascript
labelKey = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.matchPos"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>matchPos ()](#apidoc.element.react-select.propTypes.matchPos)
- description and source-code
```javascript
matchPos = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.matchProp"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>matchProp ()](#apidoc.element.react-select.propTypes.matchProp)
- description and source-code
```javascript
matchProp = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.multi"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>multi ()](#apidoc.element.react-select.propTypes.multi)
- description and source-code
```javascript
multi = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.name"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>name ()](#apidoc.element.react-select.propTypes.name)
- description and source-code
```javascript
name = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.newOptionCreator"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>newOptionCreator ()](#apidoc.element.react-select.propTypes.newOptionCreator)
- description and source-code
```javascript
newOptionCreator = function () { [native code] }
```
- example usage
```shell
...
			focusedValue = focusedValue == null ? this.state.filteredOptions[0] : focusedValue;
		}
		// Add the current value to the filtered options in last resort
		var options = this.state.filteredOptions;
		if (this.props.allowCreate && this.state.inputValue.trim()) {
			var inputValue = this.state.inputValue;
			options = options.slice();
			var newOption = this.props.newOptionCreator ? this.props.newOptionCreator(inputValue) : {
				value: inputValue,
				label: inputValue,
				create: true
			};
			options.unshift(newOption);
		}
		var ops = Object.keys(options).map(function (key) {
...
```

#### <a name="apidoc.element.react-select.propTypes.noResultsText"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>noResultsText ()](#apidoc.element.react-select.propTypes.noResultsText)
- description and source-code
```javascript
noResultsText = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.onBlur"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>onBlur ()](#apidoc.element.react-select.propTypes.onBlur)
- description and source-code
```javascript
onBlur = function () { [native code] }
```
- example usage
```shell
...
			if (_this4._focusAfterUpdate) return;
			_this4.setState({
				isFocused: false,
				isOpen: false
			});
		}, 50);
		if (this.props.onBlur) {
			this.props.onBlur(event);
		}
	},

	handleKeyDown: function handleKeyDown(event) {
		event.preventDefault();
		if (this.props.disabled) return;
		switch (event.keyCode) {
...
```

#### <a name="apidoc.element.react-select.propTypes.onChange"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>onChange ()](#apidoc.element.react-select.propTypes.onChange)
- description and source-code
```javascript
onChange = function () { [native code] }
```
- example usage
```shell
...
	getInputNode: function getInputNode() {
		var input = this.refs.input;
		return this.props.searchable ? input : React.findDOMNode(input);
	},

	fireChangeEvent: function fireChangeEvent(newState) {
		if (newState.value !== this.state.value && this.props.onChange) {
			this.props.onChange(newState.value, newState.values);
		}
	},

	handleMouseDown: function handleMouseDown(event) {
		// if the event was triggered by a mousedown and not the primary
		// button, or if the component is disabled, ignore it.
		if (this.props.disabled || event.type === 'mousedown' && event.button !== 0) {
...
```

#### <a name="apidoc.element.react-select.propTypes.onFocus"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>onFocus ()](#apidoc.element.react-select.propTypes.onFocus)
- description and source-code
```javascript
onFocus = function () { [native code] }
```
- example usage
```shell
...
				this._bindCloseMenuIfClickedOutside();
			} else {
				this._unbindCloseMenuIfClickedOutside();
			}
		});
		this._openAfterFocus = false;
		if (this.props.onFocus) {
			this.props.onFocus(event);
		}
	},

	handleInputBlur: function handleInputBlur(event) {
		var _this4 = this;

		this._blurTimeout = setTimeout(function () {
...
```

#### <a name="apidoc.element.react-select.propTypes.onInputChange"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>onInputChange ()](#apidoc.element.react-select.propTypes.onInputChange)
- description and source-code
```javascript
onInputChange = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.onOptionLabelClick"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>onOptionLabelClick ()](#apidoc.element.react-select.propTypes.onOptionLabelClick)
- description and source-code
```javascript
onOptionLabelClick = function () { [native code] }
```
- example usage
```shell
...
				noResultsText
			);
		}
	},

	handleOptionLabelClick: function handleOptionLabelClick(value, event) {
		if (this.props.onOptionLabelClick) {
			this.props.onOptionLabelClick(value, event);
		}
	},

	render: function render() {
		var selectClass = classes('Select', this.props.className, {
			'is-multi': this.props.multi,
			'is-searchable': this.props.searchable,
...
```

#### <a name="apidoc.element.react-select.propTypes.optionComponent"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>optionComponent ()](#apidoc.element.react-select.propTypes.optionComponent)
- description and source-code
```javascript
optionComponent = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.optionRenderer"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>optionRenderer ()](#apidoc.element.react-select.propTypes.optionRenderer)
- description and source-code
```javascript
optionRenderer = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.options"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>options ()](#apidoc.element.react-select.propTypes.options)
- description and source-code
```javascript
options = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.placeholder"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>placeholder ()](#apidoc.element.react-select.propTypes.placeholder)
- description and source-code
```javascript
placeholder = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.searchPromptText"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>searchPromptText ()](#apidoc.element.react-select.propTypes.searchPromptText)
- description and source-code
```javascript
searchPromptText = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.searchable"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>searchable ()](#apidoc.element.react-select.propTypes.searchable)
- description and source-code
```javascript
searchable = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.searchingText"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>searchingText ()](#apidoc.element.react-select.propTypes.searchingText)
- description and source-code
```javascript
searchingText = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.singleValueComponent"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>singleValueComponent ()](#apidoc.element.react-select.propTypes.singleValueComponent)
- description and source-code
```javascript
singleValueComponent = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.value"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>value ()](#apidoc.element.react-select.propTypes.value)
- description and source-code
```javascript
value = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.valueComponent"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>valueComponent ()](#apidoc.element.react-select.propTypes.valueComponent)
- description and source-code
```javascript
valueComponent = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.valueKey"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>valueKey ()](#apidoc.element.react-select.propTypes.valueKey)
- description and source-code
```javascript
valueKey = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.valueRenderer"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>valueRenderer ()](#apidoc.element.react-select.propTypes.valueRenderer)
- description and source-code
```javascript
valueRenderer = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.propTypes.addLabelText"></a>[module react-select.propTypes.addLabelText](#apidoc.module.react-select.propTypes.addLabelText)

#### <a name="apidoc.element.react-select.propTypes.addLabelText.addLabelText"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>addLabelText ()](#apidoc.element.react-select.propTypes.addLabelText.addLabelText)
- description and source-code
```javascript
addLabelText = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.addLabelText.isRequired"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.addLabelText.</span>isRequired ()](#apidoc.element.react-select.propTypes.addLabelText.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.propTypes.allowCreate"></a>[module react-select.propTypes.allowCreate](#apidoc.module.react-select.propTypes.allowCreate)

#### <a name="apidoc.element.react-select.propTypes.allowCreate.allowCreate"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>allowCreate ()](#apidoc.element.react-select.propTypes.allowCreate.allowCreate)
- description and source-code
```javascript
allowCreate = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.allowCreate.isRequired"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.allowCreate.</span>isRequired ()](#apidoc.element.react-select.propTypes.allowCreate.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.propTypes.asyncOptions"></a>[module react-select.propTypes.asyncOptions](#apidoc.module.react-select.propTypes.asyncOptions)

#### <a name="apidoc.element.react-select.propTypes.asyncOptions.asyncOptions"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>asyncOptions ()](#apidoc.element.react-select.propTypes.asyncOptions.asyncOptions)
- description and source-code
```javascript
asyncOptions = function () { [native code] }
```
- example usage
```shell
...
					this.setState(newState);
					if (callback) callback.call(this, newState);
					return;
				}
			}
		}

		this.props.asyncOptions(input, function (err, data) {
			if (err) throw err;
			if (_this6.props.cacheAsyncResults) {
				_this6._optionsCache[input] = data;
			}
			if (thisRequestId !== _this6._currentRequestId) {
				return;
			}
...
```

#### <a name="apidoc.element.react-select.propTypes.asyncOptions.isRequired"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.asyncOptions.</span>isRequired ()](#apidoc.element.react-select.propTypes.asyncOptions.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.propTypes.inputProps"></a>[module react-select.propTypes.inputProps](#apidoc.module.react-select.propTypes.inputProps)

#### <a name="apidoc.element.react-select.propTypes.inputProps.inputProps"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>inputProps ()](#apidoc.element.react-select.propTypes.inputProps.inputProps)
- description and source-code
```javascript
inputProps = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.inputProps.isRequired"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.inputProps.</span>isRequired ()](#apidoc.element.react-select.propTypes.inputProps.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.propTypes.options"></a>[module react-select.propTypes.options](#apidoc.module.react-select.propTypes.options)

#### <a name="apidoc.element.react-select.propTypes.options.options"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>options ()](#apidoc.element.react-select.propTypes.options.options)
- description and source-code
```javascript
options = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.options.isRequired"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.options.</span>isRequired ()](#apidoc.element.react-select.propTypes.options.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# <a name="apidoc.module.react-select.propTypes.value"></a>[module react-select.propTypes.value](#apidoc.module.react-select.propTypes.value)

#### <a name="apidoc.element.react-select.propTypes.value.value"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.</span>value ()](#apidoc.element.react-select.propTypes.value.value)
- description and source-code
```javascript
value = function () { [native code] }
```
- example usage
```shell
n/a
```

#### <a name="apidoc.element.react-select.propTypes.value.isRequired"></a>[function <span class="apidocSignatureSpan">react-select.propTypes.value.</span>isRequired ()](#apidoc.element.react-select.propTypes.value.isRequired)
- description and source-code
```javascript
isRequired = function () { [native code] }
```
- example usage
```shell
n/a
```



# misc
- this document was created with [utility2](https://github.com/kaizhu256/node-utility2)
