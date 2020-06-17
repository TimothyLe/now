![now](https://assets.zeit.co/image/upload/v1581518533/repositories/now-cli/v4.png)
[![Join the community on GitHub Discussions](https://badgen.net/badge/join%20the%20discussion/on%20github/black?icon=github)](https://github.com/zeit/now/discussions)

### <span style="color:red"> DEBUG NOTES </span>

Command from docs to install now

```sh
npm i -g now
```

Result after invoking `now`

```
~/AppData\Roaming\npm/node_modules/node/bin/node: line 1: This: command not found
```

Contents of the `node` file

```
This file intentionally left blank
```

Note: The yarn installation of `now` works properly on the command line but the npm version fails. Both `now` scripts for yarn and npm can be found in `/debug`

**TEMPORARY SOLUTION**: Add `<YOUR_DIRECTORY>/now/packages/now-cli/scripts/start.js` to your \$PATH variable or ~/.bashrc as an alias

## Usage

To quickly start a new project, run the following commands:

```
now init        # Pick an example project
cd <PROJECT>    # Change directory to the new project
now             # Deploy to the cloud
```

## Documentation

For details on how to use Now CLI, check out our [documentation](https://vercel.com/docs).
