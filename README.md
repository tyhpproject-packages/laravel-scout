<!-- tyhp-readme:start -->
# tyhpdef/laravel-scout

Tyhp type definitions for `laravel/scout` `11.7.0`.

```bash
composer require --dev tyhpdef/laravel-scout:11.7.0
```

This is a metapackage. Composer also installs `tyhpdef/laravel-scout-impl` (type files).
Require **this** name, not `tyhpdef/laravel-scout-impl`.

See https://tyhplang.com.

## Maintain `laravel/scout`? Ship the types yourself

If you are a Packagist maintainer of `laravel/scout`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/laravel-scout-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `laravel/scout` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/laravel-scout": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `laravel/scout` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `laravel/scout` with a real constraint,
   `"replace": { "tyhpdef/laravel-scout": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `laravel/scout` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/laravel-scout` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
