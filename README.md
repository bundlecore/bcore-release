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
##### Remember to replace vX.Y.Z to your desired version. 
 - Using `curl`
  ```bash
  curl -L \
    https://github.com/bundlecore/bcore-release/releases/download/vX.Y.Z/bcore-linux-amd64 \
    -o bcore-linux-amd64
```

  - Using `wget`
  ```bash
  wget https://github.com/bundlecore/bcore-release/releases/download/vX.Y.Z/bcore-linux-x64
  ```
  - Install to your local bin or path
  ```bash 
  sudo mv bcore-linux-amd64 /usr/local/bin/bcore
  ```

#### Verifying checksums
```bash
# Download checksums
curl -LO https://github.com/bundlecore/bcore-release/releases/download/v1.0.11-qa/checksums.txt

# Verify checksums (Linux)
sha256sum -c checksums.txt

# Verify specific file
sha256sum -c checksums.txt | grep bcore-linux-x64
```
The output should report `OK` for the binary you downloaded.

## Features
- List installed tools and manage versions
- Install, upgrade, and uninstall containerized tools
- Apptainer/Singularity container support
- Interactive and non-interactive CLI modes
- Global options: --version, --help
- Configuration management
