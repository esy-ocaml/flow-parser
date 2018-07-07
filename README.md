# `flow-parser` 

[![Build Status](https://travis-ci.org/esy-ocaml/flow-parser.svg?branch=master)](https://travis-ci.org/esy-ocaml/flow-parser)

Flow is a static typechecker for JavaScript. To find out more about Flow, check out [flow.org](https://flow.org/).

This project is simply a repackaging of the Flow parser as an `esy` package for
easy distribution on npm. Normally, there wouldn't be any need for this
package, but here's why this exists:

- Flow doesn't release new versions to opam frequently enough. It's very easy
  to make a new easy package that is more up to date and released to npm as an
  esy package.
- Flow's release has a misconfigured META file.
- This version makes use of dune namespacing to avoid module conflicts.


## Consume As Library:
To consume this as a library, just add `"@esy-ocaml/flow-parser"` as a
dependency of your esy project.


## To Build / Test `flow-parser` Locally:

You need Esy, you can install the beta using [npm][]:

    % npm install -g esy@preview

Then you can install the project dependencies using:

    % esy install

Then build the project dependencies along with the project itself:

    % esy build

And test compiled executable: `esy x` lets you run built binaries by name.

    % esy x TestFlow.exe


## License
Flow is MIT-licensed ([LICENSE](http://github.com/facebook/flow/blob/master/LICENSE)). The [website](https://flow.org/) and [documentation](https://flow.org/en/docs/) are licensed under the Creative Commons Attribution 4.0 license ([website/LICENSE-DOCUMENTATION](https://github.com/facebook/flow/blob/master/website/LICENSE-DOCUMENTATION)).

