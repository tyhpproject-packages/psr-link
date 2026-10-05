<!-- tyhp-readme:start -->
# tyhpdef/psr-link

Tyhp type definitions for `psr/link` `2.0.1`.

```bash
composer require --dev tyhpdef/psr-link:2.0.1
```

This is a metapackage. Composer also installs `tyhpdef/psr-link-impl` (type files).
Require **this** name, not `tyhpdef/psr-link-impl`.

See https://tyhplang.com.

## Maintain `psr/link`? Ship the types yourself

If you are a Packagist maintainer of `psr/link`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/psr-link-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `psr/link` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/psr-link": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `psr/link` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `psr/link` with a real constraint,
   `"replace": { "tyhpdef/psr-link": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `psr/link` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/psr-link` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
