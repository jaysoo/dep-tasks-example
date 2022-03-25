Example showing dependency tasks.

Running:

```
nx build a
```

Should run `codegen` for `b` and `c`, but it only does it for `b`.

```
 >  NX   Running target build for project a and 1 task(s) it depends on

 —————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————

> nx run b:codegen

>>> codegen b

> nx run a:build

>>> build a

 —————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————————

 >  NX   Successfully ran target build for project a
```
