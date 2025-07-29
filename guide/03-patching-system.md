# 03. Patching the System

1. Extract all your images into a folder (e.g., `crb`).
2. Inside `system`, delete every `my_*` folder.
3. Copy the `my_*` partitions from your images into the root of `system`.
4. Open `my_manifest/build.prop`:
   - Delete `first.api` line
   - Set your device in `market.name`
5. Add `apex` folder to `system_ext/apex`
6. Copy any overlays into `my_product`
7. In `my_product/build.prop`:
   - Change `oplusrom.display` to include your name (e.g., `15.0 | by YOURNAME`)
   - Delete any `screenhole` line
   - Find `lcd.density` and set to 440 (or as needed)
   - Remove lines starting with:
     - `ro.density.screenzoom.fdh`
     - `ro.density.screenzoom.qdh`
     - `ro.oplus.density.fhd_default`
     - `ro.oplus.density.qhd_default`
     - `ro.oplus.resolution.low`
     - `ro.oplus.resolution.high`
8. In `system/build.prop`, add:
   - `import /my_bigball/build.prop`
   - `import /my_carrier/build.prop`
   - `import /my_engineering/build.prop`
   - `import /my_heytap/build.prop`
   - `import /my_manifest/build.prop`
   - `import /my_product/build.prop`
   - `import /my_region/build.prop`
   - `import /my_stock/build.prop`
