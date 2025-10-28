# LegacyControlPanel

A curated set of verified shortcuts to classic Control Panel items, scripting tools, and legacy Windows utilities — fully compatible with **Windows 10 and 11**, including **version 25H2**.

---

## 🧭 What's Included

- ✅ Desktop `.lnk` shortcuts to hidden or deprecated Control Panel items  
- 🖼️ Icon index references from `shell32.dll`, `imageres.dll`, and `WFS.exe`  
- 📋 CLSIDs, Run commands, and scripting paths  
- 🧠 Compatibility notes and fallback options  

## 🖥️ Compatibility

Tested and confirmed working on:

- **Windows 10** — all versions from 1607 to 22H2  
- **Windows 11** — all versions from 21H2 to **25H2**  

Some legacy items (e.g., *Scanners and Cameras*) may require compatible hardware or drivers to appear.

---

## 📂 Folder Structure

```\
LegacyControlPanel/
├── Shortcuts/           # Verified .lnk files
├── Icons/               # PNG previews of icon indices
├── Reference/           # CLSIDs, commands, and icon index maps
└── LICENSE              # MIT License
\```

## 🛠️ Setup Instructions

1. Clone or download this repository  
2. Copy `.lnk` files from `/Shortcuts` to your desktop or Start Menu  
3. Right-click each shortcut → **Properties** → **Change Icon**  
4. Use icon sources like:
   - `shell32.dll`
   - `imageres.dll`
   - `WFS.exe`

---

## 📋 Example Shortcuts

| Name                         | Target Command                                                  | Icon Source             |
|------------------------------|------------------------------------------------------------------|--------------------------|
| Scanners and Cameras         | `control /name Microsoft.ScannersAndCameras`                    | `shell32.dll,134`        |
| Windows Media Player Legacy | `wmplayer.exe`                                                  | `wmploc.dll,0`           |
| PowerShell                   | `powershell.exe`                                                | `powershell.exe`         |
| PowerShell (x86)            | `%SystemRoot%\SysWOW64\WindowsPowerShell\v1.0\powershell.exe`  | `powershell.exe`         |
| PowerShell ISE              | `powershell_ise.exe`                                            | `powershell_ise.exe`     |
| PowerShell ISE (x86)        | `%SystemRoot%\SysWOW64\WindowsPowerShell\v1.0\powershell_ise.exe` | `powershell_ise.exe`  |

## 📄 License

This project is licensed under the [MIT License](LICENSE).

You are free to use, modify, and distribute the contents of this repository under the terms of the MIT License. See the LICENSE file for full details.

---

## 🙌 Contributions

Pull requests are welcome! If you have additional shortcuts, icon references, or compatibility notes, feel free to contribute.

To contribute:

1. Fork the repository  
2. Create a new branch (`git checkout -b feature-name`)  
3. Commit your changes (`git commit -am 'Add new shortcut'`)  
4. Push to the branch (`git push origin feature-name`)  
5. Open a pull request
