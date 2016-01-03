CoffeeScript Source
===================

This repository contains a basic [Crystal](http://crystal-lang.org) shard that contains the raw javascript for the [CoffeeScript](https://github.com/jashkenas/coffeescript) compiler. This shard's version will directly match the version of the corresponding CoffeeScript compiler.

Most of this code was taken from Ruby's [coffee-script-source](https://rubygems.org/gems/coffee-script-source)'s gem and Crystalized.

Installation
============

In your `shard.yml`:

```yaml
dependencies:
  coffee-script-source:
    github: jessedoyle/coffee-script-source
    version: ~> 1.10.0
```

the execute `shards install`.

Usage
=====

```crystal
require "coffee-script-source"

CoffeeScript::Source.bundled_path # => somewhere...
```

Maintenance
===========

For future reference, when a new CoffeeScript version is released:

1. Create a new branch on this repo, then checout the created branch.
2. From the repo's root directory execute: `bin/build-coffee-script 1.x.x`.
3. Commit and merge as usual. Don't forget to add the correct release tags (eg. `v1.10.0`).

License
=======

The MIT License. See `LICENSE.md` for details.