# Using one TS lib in another inside monorepo

This is part of the answer for SO question [How do I use the tsconfig.json "types" field when in a monorepo?](https://stackoverflow.com/questions/73262618/how-do-i-use-the-tsconfig-json-types-field-when-in-a-monorepo)

## Getting started

1. clone this repo
2. run `npm ci` in the root folder (no need to install/link libraries A and B)
3. `cd library-b && tsc --noEmit` - observe no errors

The library-b uses both `someGlobalFunction()` from the library-a type definitions, and `const LIB_A` from regular exports of the library-a
