# wth-php

Static PHP builds for macOS on Apple Silicon, consumed by the wth app. Each release tag `php-X.Y.Z` carries:

* `php-X.Y.Z-cli-macos-aarch64.tar.gz` (the `php` binary)
* `php-X.Y.Z-fpm-macos-aarch64.tar.gz` (the `php-fpm` binary)
* `xdebug-X.Y.Z-macos-aarch64.tar.gz` (xdebug as a shared extension, loaded with `zend_extension=`)
* `php-X.Y.Z-modules.txt`

Built with [static-php-cli](https://github.com/crazywhalecc/static-php-cli) and the extension list in `extensions.txt`. The workflow runs weekly to pick up patch releases, and on demand with a custom version list.
