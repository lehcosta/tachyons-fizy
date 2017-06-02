# fizy-tachyons

This project is an **extension** of [tachyons](https://github.com/tachyons-css/tachyons).
Files in `src/` add or redefine classes in `tachyons`, and the final built files bundle the original `tachyons`

## How to develop

### Local Setup

clone the repo from bitbucket and install dependecies through `yarn`.

```
git clone git@bitbucket.org:fizy-team/fizy-tachyons.git
cd fizy-tachyons
yarn install
```

### Dev

If you want to just use everything in tachyons/src as a jumping off point and
edit all the code yourself, you can compile all of your wonderful changes by
running

```
yarn start
```

This will output both minified and unminified versions of the css to the css directory and watch the src directory for changes.
It's aliased to the command:

```
npm run build:watch
```

If you'd like to just build the css once without watching the src directory run

```
npm run build
```

If you want to check that a class hasn't been redefined or 'mutated' there is a linter to check that all of the classes have only been defined once. This can be useful if you are using another library or have written some of your own css and want to make sure there are no naming collisions. To do this run the command

```
npm run mutations
```