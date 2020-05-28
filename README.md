# amf-named-example-in-optional-query-param-in-overlay-bug-repo

This repo reproduces [an issue in AMF-client-js](https://github.com/aml-org/amf/issues/590) where defining a named example on an optional query parameter in an overlay RAML fails AMF validation.

[Docs on AMF Validation](https://github.com/mulesoft-labs/amf-validation-example/blob/master/documentation/validation.md)

## To Run

`npm start`

The current output will look like:

```sh
$ npm start

> amf-named-example-in-optional-query-param-in-overlay-bug-repo@1.0.0 start /Users/wpeter/Source/Repos/amf-named-example-in-optional-query-param-in-overlay-bug-repo
> node index.js

Found 1 violation(s) when using RAML validator:
validationId: http://a.ml/vocabularies/amf/core#resolution-validation ::: message: Property 'http://a.ml/vocabularies/apiContract#required' in 'Parameter' is not allowed to be overriden or added in overlays
Complete
```

## To Debug

Use the checked-in vscode debug profile (just hit F5 in vscode). Or `node --inspect-brk index.js` and attach.
