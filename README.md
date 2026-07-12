# DiggaOS

<p align="center">
  <b>The ultra-minimalist, shell-only OS built to run on mobile emulators.</b>
</p>

---

### About
DiggaOS is a bare-bones, x86_64 Linux environment. No GUI, no bloat, just you and the kernel. Built automatically via GitHub Actions, it is designed to boot in seconds on lightweight environments like Limbo or v86.

### Booting the System
1. **Download:** Grab the latest diggaos.iso from the Actions tab.
2. **Setup Limbo:**
   - Machine Type: pc
   - CPU: qemu64
   - RAM: 512MB or 1024MB
   - CDROM: Select your diggaos.iso
3. **Fire it up.**

### Architecture
- Kernel: Dynamically pulled from host environment.
- Init: Custom script with static BusyBox.
- Bootloader: GRUB 2 (Text-only mode).
- Persistence: Supports external disk mounting via /dev/sda1.

### The Identity
```text
  ____  _                      ____   ____  
 |  _ \(_) __ _  __ _  __ _   / __ \ / ___| 
 | | | | |/ _` |/ _` |/ _` | | |  | |\___ \ 
 | |_| | | (_| | (_| | (_| | | |__| | ___) |
 |____/|_|\__, |\__, |\__,_|  \____/ |____/ 
          |___/ |___/                       
