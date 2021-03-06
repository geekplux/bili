# Bili

Delightful library bundler.

## Features

- 🚀 Fast, zero-config by default.
- 📦 Using Rollup under the hood.
- 🚗 Automatically transforms JS files using Buble/Babel/TypeScript.
- 💅 Built-in support for `CSS` `Sass` `Stylus` `Less` `CSS modules`.
- 🎶 Ridiculously easy to use Rollup plugins if you want.
- 🚨 Friendly error logging experience.

## Quick Start

Run a single command to bundle `src/index.js`:

```bash
bili
```

And the output will be:

```
┌───────────────────────────────────┐
│file               size   gzip size│
│dist/index.cjs.js  84 B   98 B     │
└───────────────────────────────────┘
```

It's bundled into CommonJS format by default, to bundle in multiple formats at the same time you can use the [`format`](/options#format) option:

```bash
bili --format cjs,umd,umd-min
```

- `dist/index.cjs.js`: CommonJS format, to use in Node.js or with a bundler.
- `dist/index.js`: UMD format, to use in browser directly.
- `dist/index.min.js`: UMD format, to use in browser directly.
- `dist/index.es.js`: ES modules format.

You may use a custom [`moduleName`](/options#modulename) for the UMD format.
