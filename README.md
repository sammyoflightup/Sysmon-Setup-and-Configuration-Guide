## Sysmon – System Monitoring for Windows

### What is Sysmon?

Sysmon (System Monitor) is a Windows system-level monitoring utility from Microsoft Sysinternals. It runs as a background service and logs detailed information about:

- Process creations
- Network connections
- File creation time changes
- Driver and image loading
- And more

These logs are sent to the Windows Event Log under `Applications and Services Logs > Microsoft > Windows > Sysmon`.

---

### 📦 Prerequisites

- Windows 10 or later
- Administrator privileges
- [Download Sysmon](https://learn.microsoft.com/en-us/sysinternals/downloads/sysmon)

---

### 📁 Step-by-Step Installation Using Default Configuration

1. **Extract Sysmon**
   - Unzip the downloaded Sysmon zip file.
   - Copy the folder to `C:\Program Files\Sysmon` (or any directory, but `Program Files` is ideal for persistence).

2. **Open PowerShell as Administrator**
   - Right-click Start > Windows PowerShell (Admin)

3. **Navigate to Sysmon Folder**
4. Install Sysmon with Default Configuration
   .\Sysmon64.exe -accepteula -i

   ```powershell
   cd "C:\Program Files\Sysmon"
