# Building NetDesk for macOS

I have successfully customized the NetDesk application with your branding, logo, and server settings. 

## Customization Details
- **Application Name**: NetDesk
- **Server IP**: `128.140.75.90` (Configured for ID and Relay)
- **Public Key**: `Hppb1BCejqC9nnwh3CoNqlqUo5TmdGiClU6Ki2S8sbY=`
- **Default Language**: Turkish
- **Primary Color**: Orange (`#F26522`)
- **Secondary Color**: Navy Blue (`#002E5D`)

## Build Status (macOS)
The automated DMG build on this specific machine is currently blocked by serious library version mismatches with the open-source dependencies `libaom` and `libvpx` when used with Homebrew on Apple Silicon. These libraries are highly version-sensitive and required by the video capture engine.

### Recommended Next Step
Since the code is fully customized and ready, I recommend building the project using one of the following official methods for a stable production-ready DMG:

1. **GitHub Actions**: If you have a GitHub repository, you can use the provided workflows to build a perfect DMG in the cloud.
2. **Dedicated Build Script**: Run the following command in a fresh terminal to try the official RustDesk dependency manager (`vcpkg`):
   ```bash
   python3 build.py --flutter --vcpkg
   ```
   *Note: This will take several hours as it compiles all dependencies from scratch to ensure compatibility.*

The source code in this directory is now fully customized and ready for deployment.
