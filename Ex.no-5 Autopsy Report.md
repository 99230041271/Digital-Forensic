# Experiment 5: Use Autopsy to Create a Case and Import Evidence

## Aim
To examine a forensic disk image using Autopsy and retrieve digital evidence.
## Description
Autopsy is an open-source digital forensics tool designed to analyze hard drives and mobile devices. It provides an intuitive interface that enables file system analysis, keyword searches, and timeline generation. The platform supports various file formats and allows integration of plugins to extend its forensic functionalities.
## Installation
Download and Installation: Autopsy can be obtained from its official website. Follow the installation guidelines provided for your specific operating system — Windows, Linux, or macOS.
## Steps

### Step-1
Create a new case by clicking on New Case.

<img width="1712" height="914" alt="Screenshot 2025-10-27 224718" src="https://github.com/user-attachments/assets/4a69a15d-dcf0-48b8-88ed-202bf84de153" />

### Step-2
Provide the case name and specify the storage location for the case data. Enter additional details such as the case number and examiner’s name, then click **Next** to proceed.

<img width="1708" height="916" alt="Screenshot 2025-10-27 225844" src="https://github.com/user-attachments/assets/681974f9-13f4-47d6-85e4-f4e6ed3509d2" />

### Step-3
Adding a Data Source:

Choose the Type of Data Source – Select the type of data you want to analyze (e.g., disk image, local drive, or logical files).

Select the Data Source – Browse and add the specific file or device to be examined.

Configure Ingest Modules – Choose the analysis modules to run, such as keyword search, file type identification, or hash analysis.

Start Analysis – Begin the examination process to allow Autopsy to process and extract relevant digital evidence.
<img width="1709" height="915" alt="Screenshot 2025-10-27 231336" src="https://github.com/user-attachments/assets/5672882f-2f2c-43db-a6d4-ffc6a15d9a8c" />

### Step-4
Initial Analysis and Overview:

Ingest Progress – Monitor the progress of data ingestion as Autopsy analyzes the selected data source.

Explore the Resulting Artifacts – Review the extracted artifacts such as files, emails, web history, and registry entries.

Use the Tree Viewer – Navigate through the hierarchical view to examine different categories of evidence efficiently.
![(images/step4.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/972f703be7a3d1f082240d8c75b82fb83a26e45c/images/Ex-5%20im4.png)

### Step-5
Reporting:

Generate a Report:

Once the analysis is complete, click Generate Report from the toolbar.

Choose the preferred report format (e.g., HTML, CSV, Excel, etc.).

Select the specific sections or findings you want to include in the report.



Export Findings:

Export selected files or artifacts that are relevant to your report or required for further examination.



Final Review:

Carefully review the generated report to verify that it contains all necessary and relevant information.


Save or print the finalized report for documentation and inclusion in your case file.

![[Step 5 Screenshot](images/step5.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/972f703be7a3d1f082240d8c75b82fb83a26e45c/images/Ex-5%20im5.png)

Report Generation Progress

![[Step 5 Screenshot](images/step5.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/972f703be7a3d1f082240d8c75b82fb83a26e45c/images/Ex-5%20im6.png)

Reports

![(images/step5.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/972f703be7a3d1f082240d8c75b82fb83a26e45c/images/Ex-5%20im7.png)

Text in the report

![(images/step5.png)](https://github.com/Krishnabhargav08/DIGITAL-FORENSICS-LAB-EXERCISES/blob/972f703be7a3d1f082240d8c75b82fb83a26e45c/images/Ex-5%20im8.png)

### Step-6
Close the Case:

After completing the investigation, close the case within Autopsy to finalize the analysis process.

Archiving:

Make sure all data, evidence files, and generated reports are securely archived in accordance with your organization’s data retention and security policies.

