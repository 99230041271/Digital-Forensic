# Ex.No.4   MHA (Mail Header Analyzer)
## Aim :
- The aim is to use a Mail Header Analyzer (MHA) to trace an email's origin and verify its authenticity by examining its header for signs of spoofing.
## Procedure
### Step 1: Get the Email Header
- First, you need to copy the full, raw header from the email.

- Gmail: Open the email, click the three dots (⋮), and select Show original.
<br>
<img width="1859" height="945" alt="Screenshot 2025-09-01 212142" src="https://github.com/user-attachments/assets/f7e8ee3e-1af0-46b4-b3da-da833d90f295" />
<br>
- Select all the text in the header and copy it.

<br>
<img width="1505" height="919" alt="Screenshot 2025-09-01 212318" src="https://github.com/user-attachments/assets/28e3b6d8-f667-444a-bb3d-c45f1911d4e5" />

<br>
<br>

### Step 2: Use a Mail Header Analyzer (MHA)
- The easiest way to analyze the header is with an online tool.

- Navigate to a site like MXToolbox Email Header Analyzer.
 <br>
<br>

<img width="1919" height="901" alt="Screenshot 2025-09-01 212349" src="https://github.com/user-attachments/assets/672d3f77-1c2f-413e-964c-ea3b7ce45bb4" />

<br>
<br>

- Paste the entire header you copied into the analysis box.
<br>
<br>

Click the "Analyze" button to get a parsed, easy-to-read report.
<br>
<br>

<img width="1917" height="903" alt="Screenshot 2025-09-01 212430" src="https://github.com/user-attachments/assets/9c73b860-36ab-4c19-9440-4f855fc42056" />

### Step 3: Analyze The Report
- This is the most critical step. In the analyzer's report, look for the SPF, DKIM, and DMARC results.
### Review the Overall Delivery Summary
- First, look at the high-level summary to get an immediate sense of the email's status.

- Check DMARC Compliance: The report shows the email is DMARC Compliant. This is the most important overall result.

- Check SPF Status: Both SPF Authenticated and SPF Alignment passed. This means the sending server was authorized.

- Check DKIM Status: DKIM Alignment passed, but DKIM Authenticated failed (❌). This is a critical finding and indicates a problem with the email's digital signature.
<br>
<br>
<img width="1905" height="904" alt="Screenshot 2025-09-01 212502" src="https://github.com/user-attachments/assets/8c992527-f843-48a8-9e17-63e974b8e2d4" />


<br>
<br>

### Investigate the SPF Record and Email Path
- Next, verify why the SPF check passed.

- Examine the SPF Record: The SPF record for the domain is v=spf1 include:mailgun.org ~all. This record explicitly authorizes servers from Mailgun to send emails on its behalf.

- Trace the Relay Information: The delivery path shows the email was sent from m241-136.mailgun.net.

- Conclusion: Since the email came from a Mailgun server, which is authorized in the SPF record, the SPF check passed.
  <br>
  <br>
<img width="1900" height="908" alt="Screenshot 2025-09-01 212545" src="https://github.com/user-attachments/assets/e11899c5-4b55-4487-9792-bec3be98f36c" />

<br>
<br>

### Analyze the DKIM Failure

<br>
<img width="1872" height="555" alt="Screenshot 2025-09-01 212617" src="https://github.com/user-attachments/assets/8e78bfa0-1d0a-48b8-986f-92b42693a6ba" />
