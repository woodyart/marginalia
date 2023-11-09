# Download packages using APT

## Method 1. Download packages with dependencies

```bash
apt-get install --download-only <packages>
ls -lha /var/cache/apt/archives/*.deb
```

## Method 2. Download packages without dependencise

```bash
apt download <packages>
ls -lha *.deb
```