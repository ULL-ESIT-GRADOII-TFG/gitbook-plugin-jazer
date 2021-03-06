# Testing Gitbook Plugins

### Testing your plugin locally

Testing your plugin on your book before pushing it is possible using [npm link](https://docs.npmjs.com/cli/link).

In the plugin's folder, run:

```
$ npm link
```

`npm  link` iniside a package folder will create a globally-installed symbolic link
from `prefix/package-name` to the current folder 

Then in your book's folder:

```
$ npm link gitbook-plugin-<plugin's name>
```

### Unit testing on Travis

[gitbook-tester](https://github.com/todvora/gitbook-tester) makes it easy to write **Node.js/Mocha** unit tests for your plugins. Using [Travis.org](https://travis.org), tests can be run on each commits/tags.


