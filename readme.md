# VSCodium XBPS Package
This repository provides a `template` file to help you easily install `vscodium` on your `Void Linux`.

## Installation
1. Clone the repository to your computer using:
   ```bash
   git clone https://github.com/k1114linux/xbps-src-vscodium.git codium
   ```
2. Copy the `codium` directory into the `srcpkgs/` directory of your `void-packages` repository:
   ```bash
   cp -rf codium /path/to/void-packages/srcpkgs/
   ```
3. Build the package from within the `void-packages` repository:
   ```bash
   ./xbps-src pkg -f codium
   ```
4. Install the package using `xbps-install`, pointing to the `hostdir/binpkgs` repository:
   ```bash
   sudo xbps-install --repository=hostdir/binpkgs codium
   ```
5. After installation, you can launch the `codium` browser directly from your terminal using:
   ```bash
   codium
   ```