1. Install dependencies: `yarn install`.
2. Attempt to build `yarn build`.
3. Get error:

```
yarn run v1.22.19
warning package.json: No license field
$ vite build
vite v3.0.5 building for production...
✓ 736 modules transformed.
'request' is not exported by __vite-browser-external, imported by node_modules/@aws-sdk/client-cloudwatch-logs/node_modules/@aws-sdk/credential-provider-imds/dist/es/remoteProvider/httpRequest.js
file: /Users/dwight/Sites/vite/node_modules/@aws-sdk/client-cloudwatch-logs/node_modules/@aws-sdk/credential-provider-imds/dist/es/remoteProvider/httpRequest.js:4:9
2: import { ProviderError } from "@aws-sdk/property-provider";
3: import { Buffer } from "buffer";
4: import { request } from "http";
            ^
5: /**
6:  * @internal
error during build:
Error: 'request' is not exported by __vite-browser-external, imported by node_modules/@aws-sdk/client-cloudwatch-logs/node_modules/@aws-sdk/credential-provider-imds/dist/es/remoteProvider/httpRequest.js
    at error (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:1858:30)
    at Module.error (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:12412:16)
    at Module.traceVariable (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:12771:29)
    at ModuleScope.findVariable (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:11423:39)
    at FunctionScope.findVariable (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:6355:38)
    at ChildScope.findVariable (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:6355:38)
    at FunctionScope.findVariable (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:6355:38)
    at ChildScope.findVariable (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:6355:38)
    at Identifier.bind (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:7422:40)
    at CallExpression.bind (file:///Users/dwight/Sites/vite/node_modules/rollup/dist/es/shared/rollup.js:5252:23)
error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```
