# Using one TS lib in another inside monorepo

<!-- markdownlint-disable MD033 -->

This is part of the answer for SO question: [How do I use the tsconfig.json "types" field when in a monorepo?](https://stackoverflow.com/questions/73262618/how-do-i-use-the-tsconfig-json-types-field-when-in-a-monorepo)

## Getting Started

- Clone the repository:
  - `git clone git@github.com:Zamiell/ts-2libs.git`
  - `cd ts-2libs`
- Install deps:
  - `npm ci`
- Observe that there are no errors when compiling:
  - `./packages/library-2/build.sh` <br>
  (this is just a wrapper for `npx tsc`)
- Check out the branch with only [one change](https://github.com/Zamiell/ts-2libs/commit/941fc43a86ac6c59ca7a4ebeca84d2317b950554):
  - `git checkout change`
- Observe that there are errors when compiling:
  - `./packages/library-2/build.sh`
