# mytestcompositeactions

# Cache Dependencies Action

This is a composite GitHub Action that caches your Node.js dependencies using the GitHub Actions cache.

## 📦 Features

- Caches `node_modules` using `actions/cache@v3`
- Skips reinstalling packages if the cache hit
- Speeds up your CI pipeline

---

## 🚀 Usage

```yaml
name: CI Pipeline

on:
  push:
    branches: [ main ]

jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v3

      - uses: cnsivakumar/mytestcompositeactions@v1
