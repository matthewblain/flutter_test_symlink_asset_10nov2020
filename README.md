# flutter_test_symlink_asset_10nov2020

This is a test of flutter and assets and symlinks and Windows.

Steps used to create this project:

1. Start with the basic project created by Android Studio.
2. Add a very simple usage of an asset.
3. Move the asset to a symlink in the filesystem.
4. Move the asset in the pubspec from an explicit filename to a wildcard.

It should work perfectly everywhere, but on Windows there may be trouble.
It turns out, this runs up to step 3 or 4. That is where it breaks.

Broken: flutter build bundle

Working: flutter test

Issue: https://github.com/flutter/flutter/issues/70269
