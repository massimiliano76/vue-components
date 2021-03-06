# Developers Guide

## Settings up Environment

To used the source code
- Run `npm dev` from the `engage-vue-components` folder to start TS watch 
- Run `npm link` from the `engage-vue-components` `package.json` folder  
- Run `npm link engage-vue-components` from the package you are developing in

- Restart of your dev server maybe required

## Adding new Components
 - Update Demo site
 - Update README
 - Update Tests

## Release Checklist

- Check the value of `main` in `package.json` is `dist/index.js`
- Run `npm run unit` Make sure all tests are run - there are no `.only` checked in
- Run `npm run build`
- Run `git commit`
- Run `npm version` [major | minor | patch | premajor | preminor | prepatch | prerelease | from-git]
- Run `git push`
- Run `npm publish`
- Verify latest version on https://www.npmjs.com/package/engage-vue-components
- Merge PR
- Create Github version