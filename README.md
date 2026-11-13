# emerald-crdroid-ota

JSON that the system Updater of the crDroid 17.0 line for **emerald** (POCO M6 Pro 4G /
Redmi Note 13 Pro 4G) reads, plus the release assets it points to.

- A phone with this build asks `https://raw.githubusercontent.com/RamDll/emerald-crdroid-ota/main/emerald.json`
  (the URL is set by `overlays/UpdaterResOverlayEmerald` in the device tree; the stock crDroid URL
  `crdroidandroid/android_vendor_crDroidOTA/17.0/emerald.json` does not exist for this device).
- The JSON lists the builds of this line newest first; each entry carries the OTA zip in the release
  assets of the matching tag.
- Written by `scripts/ota-server` of the build repository (`RamDll/emerald-crdroid`).

This is not an official crDroid build: updates come only from here, and installing anything else
over it needs a full flash. The LineageOS line of the same device publishes elsewhere
(`RamDll/emerald-ota`) and its builds are not compatible with this one.
