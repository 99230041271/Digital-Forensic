Ex.No: 9 – Using Process Explorer to Identify Suspicious Processes

---

Aim:
To use Microsoft Sysinternals Process Explorer to monitor system activities and identify suspicious or potentially malicious processes running on a Windows computer.

---

Requirements:

* Windows Operating System
* Internet Connection
* Process Explorer (Microsoft Sysinternals Suite)
* Optional: Antivirus Software such as Windows Defender or Malwarebytes

---

Description:
Process Explorer is a component of the Microsoft Sysinternals Suite.
It is a comprehensive tool used to display detailed information about all running processes in a Windows system.
The tool assists forensic investigators and system administrators in the following ways:

* Analyzing active processes and their dependencies
* Detecting suspicious or malicious behavior in real time
* Monitoring system resource usage such as CPU and memory
* Verifying the legitimacy of processes through digital signature validation

---

##  **Step-by-Step Procedure**

###  **Step 1: Download and Setup Process Explorer**
1. Visit: 🔗 [Microsoft Sysinternals – Process Explorer](https://learn.microsoft.com/en-us/sysinternals/downloads/process-explorer)  
2. Click **Download Process Explorer**.  
3. Extract the ZIP file to a folder.  
4. Right-click `procexp64.exe` → Select **Run as Administrator**.  

---

###  **Step 2: Understanding the Interface**
1. Main window shows all running processes in a **hierarchical tree view**.  
2. Displays details like **PID**, **CPU**, **Memory**, and **Company Name**.  
3. Color Codes:
   -  **Green:** Newly started processes  
   -  **Red:** Terminated processes  
   -  **Light Blue:** Processes by current user  
   -  **Pink:** Suspended processes  

![Process Explorer Interface](https://github.com/baddiputi/Digital-Forensic-Lab-Exercises/blob/20813074f7e55b479108660a16f276f69e56ad41/images/9.1.jpeg)

---

###  **Step 3: Identify Suspicious Processes**
1. Look for **unfamiliar or oddly named processes** (e.g., `xkdjeo.exe`, `abc123.exe`).  
2. Check **Company Name** and **Description** — genuine apps show known publishers.  
3. Right-click → **Properties** → **Image Tab** → verify **Path**:
   -  Safe: `C:\Windows\System32\`
   -  Suspicious: `C:\Users\<User>\AppData\Temp\` or `Downloads\`
4. Check **Digital Signature**:
   -  Valid → Trusted  
   -  Invalid / None → Potential malware  

![Checking Process Details](https://github.com/baddiputi/Digital-Forensic-Lab-Exercises/blob/326db74a3770e2ba22207f5a48b737f17307f683/images/9.10.jpeg)

---

###  **Step 4: Analyze Process Behavior**
1. Observe **CPU**, **Memory**, and **I/O usage**.  
2. Unusual high resource usage → may indicate malware.  
3. Right-click → **Properties** → **TCP/IP Tab** to check unknown network connections.  
4. Examine **Handles** and **DLLs Tabs** for suspicious files or libraries.  

![Process Analysis](https://github.com/baddiputi/Digital-Forensic-Lab-Exercises/blob/326db74a3770e2ba22207f5a48b737f17307f683/images/9.4.jpeg)

---

###  **Step 5: Verify Process Legitimacy**
1. Google the process name — e.g., `svchost.exe` vs `svhost.exe` (typo = malware).  
2. Visit 🔗 [VirusTotal](https://www.virustotal.com) to scan or check the file.  
3. Cross-check using **ProcessLibrary.com** or official vendor websites.  

![VirusTotal Check](https://github.com/baddiputi/Digital-Forensic-Lab-Exercises/blob/326db74a3770e2ba22207f5a48b737f17307f683/images/9.6.jpeg)

---

###  **Step 6: Take Appropriate Action**
- **If Malicious:**
  - Right-click → **Kill Process**  
  - Delete the file from its directory  
- **If Unsure:**
  - Right-click → **Suspend Process** for further investigation  
- **After Removal:**
  - Perform a **Full System Scan** with antivirus tools  

![Killing Malicious Process](https://github.com/baddiputi/Digital-Forensic-Lab-Exercises/blob/326db74a3770e2ba22207f5a48b737f17307f683/images/9.8.jpeg)

---

###  **Step 7: Example Observation**
| **Detail** | **Observation** |
|-------------|----------------|
| **Process Name** | `faangpath_simple_template.pdf` |
| **CPU Usage** | 70% |
| **Path** | `C:\Users\Admin\AppData\Temp\faangpath_simple_template.pdf` |
| **Digital Signature** | None |
| **Company Name** | Unknown |
| **Network Activity** | Connected to unknown IPs |
| **Online Check (VirusTotal)** | Detected as Trojan |
| **Action Taken** | Suspended → Killed → Deleted → Full Scan Performed |

![df lab](https://github.com/user-attachments/assets/95be5212-27f2-422e-b597-bd838bd521fe)

---

##  **Result**
Using **Process Explorer**, suspicious processes were identified based on their:
- CPU usage  
- File path  
- Digital signature  
- Network activity  

Malicious processes were terminated and removed, ensuring **system integrity and security**.

---

##  **Conclusion**
**Process Explorer** is an essential forensic tool that offers detailed visibility into active processes.  
It enables cybersecurity analysts and forensic investigators to:
- **Detect** suspicious processes  
- **Analyze** resource behavior and signatures  
- **Eliminate** malicious threats effectively  

