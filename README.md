# Deno missing `Module.runMain()`

Node exports a `runMain()` function on the "module"-module. This is used in `ts-node`.

## Steps to reproduce

1. Clone this repo
2. Run `deno task build`

## Error

```sh
Task build ts-node foo.ts
error: Uncaught TypeError: Module.runMain is not a function
    at <anonymous> (file:///project/node_modules/.deno/ts-node@10.9.1/node_modules/ts-node/dist/bin.js:465:20)
```
