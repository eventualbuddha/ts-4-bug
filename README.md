## `Object is possibly 'null'` bug

This bug only appears to happen with `.js` files that are checked by TypeScript. This repo demonstrates the problem.

### Try it

```bash
$ git clone https://github.com/eventualbuddha/ts-4-bug.git
$ cd ts-4-bug
$ yarn
$ yarn tsc
```

This should work fine, but the final command yields this:

```
index.js:4:15 - error TS2531: Object is possibly 'null'.

4   console.log(a + 1);
                ~


Found 1 error.

error Command failed with exit code 2.
```
