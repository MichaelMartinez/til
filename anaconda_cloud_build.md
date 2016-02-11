# Build a Package for Anaconda Cloud / Binstar

1. Create skeleton: `conda skeleton pypi <packagename>`
2. Build the package for specific python version: `conda build --python 3.x or 2.x <packagename>`
3. Source deactivate current `env` or use "root" env
4. Login to Anaconda Cloud: `anaconda login`
5. Upload the package: `anaconda upload <packagename>`
