# 02. Extracting Images from Payload

- Get [payload-dumper-go](https://github.com/vm03/payload-dumper-go) (my go-to).
- Use 7zip to pull out `payload.bin` from your OTA zip.
- Either drag `payload.bin` onto payload-dumper-go.exe (easy) or use the command line (advanced).

You’ll get image files (`my_*`, `system`, etc.) in the folder.

> **Note:** If the tool won’t open, right-click > Run as admin.

**Now:**  
- Make an `images/` folder  
- Copy every file named:
  - `my_*`
  - `system`, `system_ext`, `product`

> *Mistake I made*: I missed one `my_bigball.img` the first time. Double-check!

---  
Next: [Patching the System](03-patching-system.md)
