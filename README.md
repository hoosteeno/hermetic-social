# Hermetic Social

An opinionated Containers addon for Firefox

[Available on addons.mozilla.org](https://example.com)

## Requirements

* node 7+ (for jpm)
* Firefox 57+

## Development

1. `npm install`
2. `./node_modules/.bin/web-ext run -s src/`

### Testing
TBD

### Distributing
#### Make the new version

1. Bump the version number in `package.json` and `manifest.json`
2. Commit the version number bump
3. Create a git tag for the version: `git tag <version>`
4. Push the tag up to GitHub: `git push --tags`

#### Publish to AMO

1. `npm run-script build`
2. [Upload the `.zip` to AMO](https://example.com)

#### Publish to GitHub
Finally, we also publish the release to GitHub for those followers.

1. Download the signed `.xpi` from [the addon versions page](https://example.com)
2. [Make the new release on
   GitHub](https://github.com/hoosteeno/hermetic-social/releases/new)
   * Use the version number for "Tag version" and "Release title"
   * Release notes: copy the output of `git log --no-merges --pretty=format:"%h %s" <previous-version>..<new-version>`
   * Attach binaries: select the signed `.xpi` file

### Links

- [Licence](./LICENSE.txt)
- [Contributing](./CONTRIBUTING.md)
- [Code Of Conduct](./CODE_OF_CONDUCT.md)
