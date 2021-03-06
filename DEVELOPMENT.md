# Development

We use [lerna](https://github.com/lerna/lerna) to publish our packages. We use the fixed versioning mode.

## Setting up the repo

```
npm install
npx lerna bootstrap
```

## Releasing

We use https://github.com/mrahhal/release-cycle as a reference when releasing.

### What changed since last release

```
npx lerna changed
```

### Update version

```
npx lerna version [version] --no-git-tag-version --no-push --yes
```

### Release

Releasing packages is handled through CI when a git version tag is pushed.

If we're updating to a version (usually a major version update) that requires updates to the peer dependencies, then use the `lerna version ...` command above to allow lerna to update what it wants to update, and then go on and update peer dependencies manually (and run `npm i` so that the lock file is updated too). After that, commit the changes, and then finally publish.
