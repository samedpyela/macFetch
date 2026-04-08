# 🍏 macFetch: The Ultimate & Most Comprehensive macOS Downloader

**macFetch** is a professional-grade, data-driven GUI utility designed specifically for the Hackintosh community, system administrators, and Apple enthusiasts. It allows you to find and download any official macOS installer or legacy image released over the last 25 years—spanning from the original **Mac OS X 10.0 Cheetah** to the latest **macOS 26 Tahoe**.

---

## 📖 What is macFetch and What Does It Do?
Finding a specific, clean macOS installer is often a nightmare. Apple hides old versions, and forums are frequently filled with dead or untrustworthy links. **macFetch** solves this by centralizing Apple's official Software Delivery Network (`swcdn.apple.com`) and community-verified links into one sleek, "Dark Mode" window.

* **Massive Library:** Support for every major release and minor "point" release (e.g., 10.15.7, 12.1, 15.0).
* **Format Options:** Download official **PKG** installers, **DMG** images, or get **BDU** (Bootable Disk Utility) links for Windows users.
* **No Coding Required:** All links are stored in an external JSON file. You can update the entire database without ever touching the Python script.
* **Cloud Sync:** Sync your local database with the latest community links from GitHub with a single click.

---

## 📦 Step 1: Installation (The Essential Setup)

To run macFetch, you must install the required libraries that power the interface and the internet features. 

**Open your Terminal (macOS/Linux) or Command Prompt (Windows) and run this exact command:**

```bash
pip3 install customtkinter requests --break-system-packages
```
---

## 🖥️ Step 2: How to Launch the App (The Correct Way)
* **IMPORTANT:** Do not just double-click the macfetch.py file! On many systems, this will simply open a text editor (like Xcode or Notepad). You must run it through the terminal to ensure it works properly.

Follow these exact steps to launch the app:

Open your Terminal (on Mac) or Command Prompt (on Windows).

Type python3  and make sure you hit the Spacebar once (so there is a space after the '3').

Locate your macfetch.py file on your Desktop or in your folder.

Drag and drop the macfetch.py file directly into the terminal window. The path to the file will appear automatically after your python3  command.

Press Enter on your keyboard.

---

## 🔄 Database Customization & GitHub Sync
macFetch is a data-driven application. It uses a file called macfetch_catalog.json (automatically created on your first launch) to manage all the download links.

1. Adding Your Own Links Manually:
Open macfetch_catalog.json with any text editor (Notepad, TextEdit, or VS Code).

Find the macOS version you want to modify (e.g., "macOS 14 Sonoma").

Replace the placeholder "YOUR_LINK_HERE" with your actual direct download URL.

Save the file and click the "🔄 Reload App" button inside the macFetch window.

2. Cloud Sync:
The app is pre-configured to sync with the official samedpyela/macFetch repository.

Simply click the "🔄 Sync GitHub" button to automatically pull the latest community-verified links into your local app instantly.

---

## ⚠️ Common Troubleshooting
Error: "ModuleNotFoundError": This means Step 1 failed. You must re-run the pip3 install command with the --break-system-packages flag.

The App Closes Immediately: Always launch via the terminal. If there is a mistake in your macfetch_catalog.json file (like a missing comma or quotation mark), the terminal will show you exactly what line is broken.

Download Button Does Nothing: Ensure the link in your JSON file is a real URL and not just placeholder text.

### Created for the community. Clean installs only. 🍏
