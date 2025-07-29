# 01. Getting OTA Files

1. **Find OTA links:**  
   - Check [ota_links/](../ota_links/) or ask around—4PDA, Telegram, or Issues tab.

2. **Download with aria2c:**  
   - Open terminal (cmd or bash) and run:
     ```
     aria2c -x16 -s16 -j5 --file-allocation=none "PASTE_OTA_LINK_HERE"
     ```
   - This is faster/more reliable than regular browser download!

> **Tip:** If your download fails, just run the same command again to resume.

---  
Next: [Extracting Images](02-extracting-images.md)
