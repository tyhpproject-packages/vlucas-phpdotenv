<!-- tyhp-readme:start -->
# tyhpdef/vlucas-phpdotenv

Tyhp type definitions for `vlucas/phpdotenv` `5.7.0`.

```bash
composer require --dev tyhpdef/vlucas-phpdotenv:5.7.0
```

This is a metapackage. Composer also installs `tyhpdef/vlucas-phpdotenv-impl` (type files).
Require **this** name, not `tyhpdef/vlucas-phpdotenv-impl`.

See https://tyhplang.com.

## Maintain `vlucas/phpdotenv`? Ship the types yourself

If you are a Packagist maintainer of `vlucas/phpdotenv`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/vlucas-phpdotenv-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `vlucas/phpdotenv` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/vlucas-phpdotenv": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `vlucas/phpdotenv` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `vlucas/phpdotenv` with a real constraint,
   `"replace": { "tyhpdef/vlucas-phpdotenv": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `vlucas/phpdotenv` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/vlucas-phpdotenv` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
