Experiment 7- Using AFLogical OSE to Extract Data from an Android Device

Aim:

To perform logical data extraction from an Android device using AFLogical OSE (Open Source Edition) and analyze the extracted data for forensic purposes.

---

Theory:

AFLogical OSE (Open Source Edition) is a component of the Open Source Android Forensics Project developed for logical acquisition of data from Android devices.
It enables investigators to collect non-destructive evidence without rooting the device.
The tool can extract essential information such as:

* Contacts
* SMS / MMS Messages
* Call Logs
* Calendar Entries
* Browser History

This method preserves data integrity and is suitable for preliminary forensic investigations.

---

Requirements:

| Hardware / Software | Description                              |
| ------------------- | ---------------------------------------- |
| System              | Windows or Linux                         |
| Device              | Android phone with USB Debugging enabled |
| Connection          | USB Cable                                |
| Tool                | AFLogical OSE                            |

---

Procedure:

1. Download and install AFLogical OSE on your system.
2. Enable Developer Options and turn on USB Debugging on the Android device.
3. Connect the device to the system using a USB cable.
4. Launch AFLogical OSE; it will automatically detect the connected device.
5. Grant the necessary permissions on the Android device when prompted.
6. Choose the data types to extract, such as Contacts, Messages, or Call Logs.
7. The tool will extract the selected data and save the results as .csv files.
8. The extracted files will be stored in the directory `/sdcard/forensics/`.
9. Copy the extracted files to your system for further forensic examination and analysis.



### 📸 Step 1 — Launching AFLogical OSE  
![Screenshot 1](https://github.com/user-attachments/assets/bf3d4690-98b2-4afc-9dcc-1b88deef2e71)

### 📸 Step 2 — Device Detection  
![Screenshot 2](https://github.com/user-attachments/assets/c16b02ed-1e48-4946-a562-043abb3e9e25)

### 📸 Step 3 — Data Extraction Process  
![Screenshot 3](https://github.com/user-attachments/assets/f84a2449-99e1-4a7f-8854-58f2964be372)

### 📸 Step 4 — Selecting Data Categories  
![Screenshot 4](https://github.com/user-attachments/assets/3bebf98b-8dab-4d04-ba44-1dc70d7d2d62)

### 📸 Step 5 — Extraction Completed  
![Screenshot 5](https://github.com/user-attachments/assets/b02f289c-3de4-42f5-90c1-518131a6e4f7)

### 📸 Step 6 — Output File Structure  
![Screenshot 6](https://github.com/user-attachments/assets/545baf69-e750-410a-b07a-657d60b91e97)

### 📸 Step 7 — Viewing Extracted Data  
![Screenshot 7](https://github.com/user-attachments/assets/22f021cb-f711-4268-88cb-eba0ed6c5684)

---

Result:

Logical data, including Contacts, Messages, and Call Logs, was successfully extracted from an Android device using AFLogical OSE.
The extracted information was saved in .csv format for further forensic analysis.

---

Conclusion:

AFLogical OSE is an effective open-source tool for performing logical data extraction in Android forensic investigations.
It allows investigators to retrieve crucial information without altering the device, making it highly suitable for preliminary forensic analysis and evidence collection.




