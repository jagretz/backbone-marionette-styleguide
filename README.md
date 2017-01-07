# (WIP) Backbone - Marionette Styleguide (WIP)

*A work in progress (wip), I have just began building an application in backbone-marionette so I am learning and gathering best practices as I go.*

## Purpose
*An opinionated backbone-marionette styleguide for teams or individuals.*

This is an opinionated style guide for syntax, conventions, and structuring backone applications using marionette library. 
If you like what you see then have at it. Have improvements to suggest, fork this or hit me up I'd love to have your suggestions!

Styles and format are based upon my very limited knowledge of and experiences while developing applications with backbone and marionette.

The intention of this styleguide is to guide projects and teams building backbone-marionette apps by showing the conventions I use and, more importantly, why the convention was chosen.

## Table of Contents

  1. [Template](#template)
  1. [Type of Object](#type-of-object)
  1. [Modules](#modules)
  1. [API References](#api-references)

## Template

- what

  *Why?*: 

```javascript
function template(param1, param2) {
    // I am a template
};
```

**[Back to top](#table-of-contents)**

## Type of Object

- Define a meta object on your backbone models, collections and views. Define additional private and immutable properties with `Object.defineProperty()`.

  *Why?*: `meta` property is a place to add meta information regarding the object.

  *Why?*: Very helpful when debugging. Provides a constructive name for your object other than `child`

  *Why?*: Makes this private and immutable.


```javascript
var ModelConstructor = Backbone.NestedModel.extend({
    meta: {}
});

Object.defineProperty(ModelConstructor.prototype.meta, 'className', {
    value: 'ModelConstructor'
});
```


**[Back to top](#table-of-contents)**

## Module

- what

  *Why?*: 

**[Back to top](#table-of-contents)**


## API References

For anything else, check the API reference:

- [Backbone documentation](http://backbonejs.org/).
- [Marionette documentation](http://marionettejs.com/docs/current/).

**[Back to top](#table-of-contents)**






