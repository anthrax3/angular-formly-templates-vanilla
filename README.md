[![Build Status](https://travis-ci.org/formly-js/angular-formly.svg)](https://travis-ci.org/formly-js/angular-formly)
[![Coverage Status](https://img.shields.io/coveralls/formly-js/angular-formly.svg)](https://coveralls.io/r/formly-js/angular-formly)

## Angular-Formly: Vanilla Template
This is a template for Angular-Formly which adds template basic files with no css classes. Each field is wrapped in a div. This library is not standalone and requires angular-formly to be present and loaded.

Example text field:
```html
	<div>
		<label for="{{id}}">
			{{options.label || 'Text'}}
			{{options.required ? '*' : ''}}
		</label>
		<input type="text"
		       id="{{id}}"
		       formly-dynamic-name="options.key"
		       formly-custom-validation="options.validators"
		       placeholder="{{options.placeholder}}"
		       aria-describedby="{{id}}_description"
		       ng-required="options.required"
		       ng-disabled="options.disabled"
		       ng-model="result[options.key || index]">
		<p id="{{id}}_description" ng-if="options.description">{{options.description}}</p>
	</div>
```

### Demo : http://formly-js.github.io/angular-formly-templates-vanilla/

## Dependencies
- Required to use Formly:
 - Angular
 - Angular-Formly

- Dev dependencies to build Formly
 - npm


See `bower.json` and `index.html` in the `master` branch for a full list / more details

## Install in your project
- Install with [Angular-Formly](https://github.com/formly-js/angular-formly)

- Install with Angular-Formly: Vanilla Templates
 `$ bower install angular-formly-templates-vanilla --save`

- Include the javascript file in your index.html, Formly comes in the following flavors:
 `<script src="bower_components/angular-formly-templates-vanilla/dist/angular-formly-templates-vanilla.min.js"></script>`

## Documentation

See [Angular-Formly](https://github.com/formly-js/angular-formly).

## Contributing

Please see the [CONTRIBUTING Guidelines](CONTRIBUTING.md).

## Thanks

A special thanks to [Nimbly](http://gonimbly.com) for creating/sponsoring Angular-Formly's development.
Thanks to [Kent C. Dodds](https://github.com/kentcdodds) for his continued support on the project.