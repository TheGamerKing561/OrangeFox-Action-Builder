# OrangeFox Action Builder
Compile OrangeFox Recovery using GitHub Actions.

# How to Use
1. Fork this repository.

2. Go to `Action` tab > `All workflows` > `OrangeFox - Build` > `Run workflow`, then fill all of the required information:
 * OrangeFox Manifest Branch (`12.1` or `14.1`.)
 * OrangeFox Device Tree (Your device tree repository link.)
 * OrangeFox Device Tree Branch (Your device tree repository branch.)
 * Device Tree Path (`device/vendor/codename`)
 * Device Codename (Your device's codename.)
 * Makefile Name (The name of your device's makefile (excluding .mk extension). Example: `twrp_codename`)
 * Build Target (depends on your device, either `boot`, `recovery`, `vendorboot`)
 * Maintainer name (The maintainer name you want to be shown in the OrangeFox build's about page.)
 * Apply custom source patches (Whether to apply custom source patches or not.)
 * Name of folder containing custom patches (The directory in which your custom source patches are located (must be inside the device tree).)

 # Note
* Currently, this action only supports 12.1 and 14.1 manifests, since all OrangeFox manifests below 12.1 are considered obsolete.
* Make sure your device tree uses the OrangeFox-specific variables too; [fox_12.1](https://gitlab.com/OrangeFox/vendor/recovery/-/blob/fox_12.1/orangefox_build_vars.txt) and [fox_14.1](https://gitlab.com/OrangeFox/vendor/recovery/-/blob/fox_14.1/orangefox_build_vars.txt).
