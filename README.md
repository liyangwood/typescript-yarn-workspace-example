## typescript-yarn-workspace-example

## Yarn v1 to v2
```
yarn set version berry
yarn set version latest
```

- https://yarnpkg.com/getting-started/install


### Add module to ./packages
```
npx lerna create @me/test_package
```

### Yarn workspaces foreach
```
yarn plugin list
yarn plugin import workspace-tools
```

### Add dependencies
```
// add to root
yarn add -W -D typescript

// add to all workspace
yarn workspaces foreach add lodash

// add to special module
yarn workspace @me/test_package add common
```



### Show workspaces info
```
yarn workspaces info
```

### Clean node_modules
```
npx lerna clean --yes
```

## Run in local
```
yarn install
yarn workspace common build
yarn workspace server start
```
