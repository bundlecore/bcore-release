# Downloading bcore CLI

This page explains how to download the **bcore** CLI binaries from the public `bcore-release` repository.

## Latest stable release

You can always find the latest stable release here:

- https://github.com/bundlecore/bcore-release/releases/latest

From that page you can download platform-specific binaries and checksums.

## Direct download URLs (by version)

Replace `vX.Y.Z` with the release version you want.

### Linux

- x86_64:

  ```bash
  curl -L \
    https://github.com/bundlecore/bcore-release/releases/download/vX.Y.Z/bcore-linux-amd64.tar.gz \
    -o bcore-linux-amd64.tar.gz

  tar -xzf bcore-linux-amd64.tar.gz
  sudo mv bcore /usr/local/bin/

#### Verifying checksums
```bash
curl -L \
  https://github.com/bundlecore/bcore-release/releases/download/vX.Y.Z/sha256sum.txt \
  -o sha256sum.txt

sha256sum --check sha256sum.txt
```
The output should report `OK` for the binary you downloaded.
