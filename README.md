# InterGenOS (Custom Fork)

> Security is not first. It is only. (And it can still be cute).

This is a personalized fork of **InterGenOS**—a Linux distribution built entirely from source based on LFS/BLFS 13.0. While it retains the core secure Forge boot chain and tiered local InterGen AI assistant from the upstream repository, this fork strips away standard components to build a lighter, highly customized user environment.

##  Fork Customizations

This fork replaces the upstream GNOME desktop defaults with tailored, alternative applications:

*   **Helium Web Browser:** Replaces standard browser helpers with the lightweight, privacy-centric Helium browser framework.
*   **so-cute-cat Terminal Engine:** Replaces GNOME Terminal with my custom `so-cute-cat` terminal i made well its an fork with added stuff 
*   **GNOME Handler Overrides:** Integrated post-install schema overrides to force GNOME to natively target `so-cute-cat` as the default system terminal application.

---

##  How to Set Up 


### Step 1: Clone and Build
Once  Ubuntu  boots up, open the **Terminal** application inside it and run the following commands:

```bash
# 1. Install Git to download the repository
sudo apt update && sudo apt install git -y

# 2. Clone this specific custom fork
git clone https://github.com/brolookslikeanfish67-hub/intergenos
cd intergenos


---

##  Upstream Core Features Retained

*   **The Forge Secure Boot Chain:** Microsoft-signed shim → MOK-signed GRUB → MOK-signed kernel → Enforced module signatures (`MODULE_SIG_FORCE=y`). 
*   **InterGen AI Assistant:** Fully offline, hardware-aware local LLM assistant (ranging from 2B to 35B parameter tiers based strictly on discrete VRAM).
*   **InterGen Sentinel:** Pluggable security-scanner architecture routing tool execution through local rule-sets and local Qwen checking.
*   **Transparent Boot:** No Plymouth boot splash. Watch the kernel hand off to systemd directly to spot compromise or misbehaving modules instantly.

---

*For full upstream licensing details (GPL-3.0), legal postures, and the core project documentation, see the original research folders or visit the upstream repository at InterGenJLU/intergenos.*
