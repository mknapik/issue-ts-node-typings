# ts-node-typings

```bash
~/w/i/ts-node-typings (master|…) ♮ yarn working
yarn run v1.9.4
$ npm run compile && npm run js

> ts-node-typings@1.0.0 compile /Users/user/workspace/iot/ts-node-typings
> tsc -p .


> ts-node-typings@1.0.0 js /Users/user/workspace/iot/ts-node-typings
> node dist/index.js

2
✨  Done in 2.10s.
```

```bash
~/w/i/ts-node-typings (master|…) ♮ yarn not:working
yarn run v1.9.4
$ npm run ts

> ts-node-typings@1.0.0 ts /Users/user/workspace/iot/ts-node-typings
> ts-node src/index.ts


/Users/user/workspace/iot/ts-node-typings/node_modules/ts-node/src/index.ts:261
    return new TSError(diagnosticText, diagnosticCodes)
           ^
TSError: ⨯ Unable to compile TypeScript:
src/index.ts(1,24): error TS2307: Cannot find module 'Types'.

    at createTSError (/Users/user/workspace/iot/ts-node-typings/node_modules/ts-node/src/index.ts:261:12)
    at getOutput (/Users/user/workspace/iot/ts-node-typings/node_modules/ts-node/src/index.ts:367:40)
    at Object.compile (/Users/user/workspace/iot/ts-node-typings/node_modules/ts-node/src/index.ts:558:11)
    at Module.m._compile (/Users/user/workspace/iot/ts-node-typings/node_modules/ts-node/src/index.ts:439:43)
    at Module._extensions..js (internal/modules/cjs/loader.js:700:10)
    at Object.require.extensions.(anonymous function) [as .ts] (/Users/user/workspace/iot/ts-node-typings/node_modules/ts-node/src/index.ts:442:12)
    at Module.load (internal/modules/cjs/loader.js:599:32)
    at tryModuleLoad (internal/modules/cjs/loader.js:538:12)
    at Function.Module._load (internal/modules/cjs/loader.js:530:3)
    at Function.Module.runMain (internal/modules/cjs/loader.js:742:12)
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! ts-node-typings@1.0.0 ts: `ts-node src/index.ts`
npm ERR! Exit status 1
npm ERR!
npm ERR! Failed at the ts-node-typings@1.0.0 ts script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
npm ERR!     /Users/user/.npm/_logs/2018-09-15T12_10_32_779Z-debug.log
error Command failed with exit code 1.
info Visit https://yarnpkg.com/en/docs/cli/run for documentation about this command.
```
