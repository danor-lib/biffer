# CHANGELOG

## v3.2.1 - 2026.05.26 16
* docs: **IMPORTANT!** update license to ***MIT***
* docs: add refactoring note in README
* docs: improve error code reference table


## v3.2.0 - 2026.05.25 16
* refactor!: due to a change in design philosophy, remove all error message text
  * in my design philosophy, an error should only contain a code and associated data. text-based message should be rendered by the terminal (including i18n and terminal highlighting)
* docs: add error code reference table
* regular!: bump up Node.js requirement to `>=26`
  * this requirement does not mean the library cannot run on older versions of Node.js. it only indicates the major version I am currently using
* regular: bump up dependencies
  * bump up `@danor-lib/error` to `v2.x`


## v3.1.0 - 2026.04.30 15
* feat: `.unpackString()` supports returning Buffer directly to provide raw data for non-UTF-8 encoded strings
* fix: fix the issue where the return value of `.unpackString()` is incorrect
* docs: tweak jsdoc style
* regular: bump up dependencies


## v3.0.1 - 2026.04.20 16
* fix: fix issue of incorrectly using the `in` operator when no option argument is passed to `#slice()`
* feat: add helper display functions `get [Symbol.toStringTag]()` and `[node:util.inspect.custom]()` inside the Biffer class to show Biffer state more conveniently
* regular: bump up dependencies


## v3.0.0 - 2026.04.17 15
* refactor!: rename package from `@nuogz/biffer` to `@danor-lib/biffer`
* refactor!: refactor `#slice()` method with new options parameter
* refactor!: remove `#sub()` method . its functionality is merged into `#slice()`
* feat: Biffer constructor to support cloning Biffer instances
* feat: add `#clone()` method to create independent Biffer instances
* refactor!: rename property `.dictSize` to `.sizes$charStruct`
* refactor!: rename property `.pos` to `.cursor`
* refactor!: rename method `.#parseChar()` to `.#parseStructChar()`
* refactor!: rename method `#findFromStart()` to `#findFromHead()`
* refactor!: rename method `#isEnd()` to `#isReach()`
* docs: completely rewrite README with detailed API documentation
* docs: add English version README.en.md
* break!: remove infrequently used `@nuogz/i18n`
* refactor: refactor error handling with `@danor-lib/error`
* feat: add `src/texter.js` for styled error messages
* regular!: bump up Node.js requirement to `>=24`
* regular: update enviroment
* regular: bump up dependencies


## v2.7.1 - 2024.08.26 11
* refactor: renew codes to adapt to latest `@nuogz/i18n`
* docs: renew locale with latest `@nuogz/i18n`
* deps: bump up dependencies


## v2.7.0 - 2024.08.23 16
* feat: new Biffer method `close()` to provide a way to close the file descriptor being used by Biffer
* refactor!: rename Biffer property `usingFileDescriptor` from `useFD`
* deps: bump up dependencies
* docs: move types into types folder
* docs: update the usage of tsc
* docs: tweak description
* chore: renew develop environments


## v2.6.0 - 2023.12.06 19
* tweak enviroment
* bump up dependencies


## v2.5.4 - 2023.04.07 09
* improve locales


## v2.5.3 - 2023.04.03 16
* fix locales typos


## v2.5.2 - 2023.04.03 16
* bump up `@nuogz/i18n` to `v3.1.0` and renew related code
* renew locales and `d.ts`


## v2.5.1 - 2023.04.03 15
* fix locales typos


## v2.5.0 - 2023.03.30 08
* bump up `@nuogz/i18n` to `v3.x` and renew related code
* renew locales and `d.ts`
* bump up dependencies


## v2.4.1 - 2023.02.01 11
* improve `d.ts`
* bump up dependencies
* fix `.npmrc` to hoist `i18next` to emit `d.ts` correctly
* improve script `emitDeclaration` to preserve symlinks in `d.ts`


## v2.4.0 - 2023.01.16 11
* support reading `float` and `double` with format `f` or `d`
* fix bug when reading char


## v2.3.0 - 2023.01.16 11
* fix unexcepted position moving when format count is `0`, like `0L`, `0c`
* improve unpacking logic
* improve comment
* bump up dependencies


## v2.2.0 - 2023.01.13 17
* add declaration files
* update `jsconfig.json`
* bump up dependencies


## v2.1.1 - 2023.01.05 10
* bump up dependencies regularly
* fix changelog


## v2.1.0 - 2022.08.12 10
* support BigInt and format `q/Q` for 8 bytes number
* improve `locale` keys and translations
* bump up `@nuogz/i18n` to `1.2.0` and update related code


## v2.0.2 - 2022.08.09 08
* change library's description
* bump up `@nuogz/i18n` to `1.0.2`
* use unified `.eslintrc.cjs` from `@nuogz/pangu`


## v2.0.1 - 2022.08.08 18
* use library `@nuogz/i18n`instead inline i18n code
* tweak `.vscode/launch.json`


## v2.0.0 - 2022.08.08 15
* start use `CHANGLOG.md` from version `v2.0.0`
* tweak all files for publishing to npm
* translate all inline documents info english
