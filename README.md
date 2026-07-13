# jsPlumb Community Edition

This project is the Community edition of jsPlumb. It is open source and MIT/GPL2 licensed. If you're looking for the Toolkit edition please visit [https://jsplumbtoolkit.com](https://jsplumbtoolkit.com).

This repository was created in October 2023 to be the new home of the original repository - [https://github.com/jsplumb/jsplumb](https://github.com/jsplumb/jsplumb).

If you're new to jsPlumb, please do take the time to read the [documentation](https://docs.jsplumbtoolkit.com/community/). 
There are a few integration issues that you should be aware of: z-index needs special attention, for example.

**This project is not the correct place to report issues for the Toolkit edition**. The Toolkit is not a public project. Issues reported for the Toolkit edition in this issue tracker will be deleted.


## Packages

In 6.x we have dispensed with the multiple packages from 5.x and we now ship a single package. If you're using a bundler with tree shaking, as the vast majority of people are nowadays, you'll get a smaller bundle size with 6.x than you did with 5.x as it is more compatible with tree shaking.

The single import for 6.x is:

```json
{
  "@jsplumb/browser-ui":"^6.0,0"
}
``` 

### What if I'm not using a package manager?

If you're not using a package manager at all then you can use the UMD that ships in the jsPlumb package.

```html
<script src="node_modules/@jsplumb/browser-ui/js/jsplumb-browser-ui.umd.js"></script>
```

---

## Documentation

For the Community edition the documentation for version 6.x is here:

[https://docs.jsplumbtoolkit.com/community/](https://docs.jsplumbtoolkit.com/community/)

For the previous versions of jsPlumb, docs are here:

[https://docs.jsplumbtoolkit.com/community/5.x](https://docs.jsplumbtoolkit.com/community/5.x)

and

[https://docs.jsplumbtoolkit.com/community/2.x](https://docs.jsplumbtoolkit.com/community/2.x)


## Issues

jsPlumb uses GitHub's issue tracker for enhancements and bugs

## Requirements

No external dependencies.

## jsPlumb in action

Links to various Community Edition demonstrations can be found [here](https://community.jsplumbtoolkit.com).

## Tests

There is a full suite of unit tests checked in to the `test` and `dist/test` directories.

## Twitter

[https://twitter.com/jsplumblib](https://twitter.com/jsplumblib)

## License

All 1.x.x, 2.x.x, 4.x.x, 5.x.x and 6.x.x versions of jsPlumb Community edition are dual-licensed under both MIT and GPLv2. 

### This fork

This repository ([kusamau/jsPlumbCommunityEdition](https://github.com/kusamau/jsPlumbCommunityEdition)) is a
fork of [jsPlumb Community Edition](https://github.com/jsplumb/community-edition). The original code's
copyright and dual MIT/GPLv2 license terms (see [`jsPlumb-LICENSE.txt`](./jsPlumb-LICENSE.txt)) are
unchanged and unremoved. Going forward, this fork elects to use and distribute its own changes under the
**MIT** license — see `CLAUDE.md` for the compliance notes that apply to any future update made here.

#### Installing this fork directly

This repository ships its built `@jsplumb/browser-ui` bundle (`dist/browser-ui`) checked in, so it can be
installed directly from GitHub as a git dependency, without a registry publish:

```json
{
  "dependencies": {
    "@jsplumb/browser-ui": "github:kusamau/jsPlumbCommunityEdition#claude/npm-installable-89glkk"
  }
}
```

or from the command line:

```
npm install github:kusamau/jsPlumbCommunityEdition#claude/npm-installable-89glkk
```

Because the installed name matches the upstream package, this is a drop-in override — existing
`import ... from '@jsplumb/browser-ui'` code keeps working unchanged. For reproducible installs, prefer
pinning to a specific commit SHA or tag instead of a branch name, e.g.
`github:kusamau/jsPlumbCommunityEdition#<commit-sha>`.
