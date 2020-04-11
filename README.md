# rfc-js-try-no-catch
A proposal for JS for `try` without `catch`/`finally`.

To silence errors for a block, we could just write this:

```js
try {
  doMaybeUnsafeThing();
}
```

Instead of one of these:

```js
try {
  doMaybeUnsafeThing();
} finally {}
```

```js
try {
  doMaybeUnsafeThing();
} catch (error) {}
```


Related:
* https://github.com/AndersDJohnson/rfc-js-catch-no-parentheses
* https://github.com/AndersDJohnson/rfc-js-try-return
