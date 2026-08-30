# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
## AIM:
To review unallocated space in a disk image, extract data using forensic tools, and understand the digital investigation process.
## REQUIREMENTS
- Autopsy or FTK Imager
- Sleuth Kit (TSK)
- Hex Editor (e.g., HxD)
- Operating System: Windows 10/11 or Linux (Kali preferred)
## ARCHITECTURE DIAGRAM
```mermaid
flowchart TD
    A[Disk Image / Physical Drive] --> B[Load into Autopsy or Sleuth Kit]
    B --> C[Identify Unallocated Space]
    C --> D[Scan for Data Signatures]
    D --> E[Carve and Recover Files]
    E --> F[Analyze Recovered Data]
    F --> G[Document Findings in Report]
```
## DESIGN STEPS:
### Step 1 (Acquire Evidence Image):
- Obtain the disk image in ```.dd``` or ```.E01``` format from a trusted forensic acquisition process.
- Verify hash values (MD5/SHA256) to maintain integrity.

### Step 2(Load Image into Forensic Tool):
- Open Autopsy or FTK Imager.
- Create a new case and add the evidence image.

### Step 3(Locate Unallocated Space):
- Navigate to the partition structure view.
- Identify sectors not assigned to any partition (unallocated).
### Step 4(Analyze & Carve Data):
- Use built-in data carving tools to search for file signatures (JPEG, DOCX, PDF, etc.).
- Preview carved files for relevance.
  
## PROGRAM:
| Step | Action                     | Tool Used                   | Output                       |
| ---- | -------------------------- | --------------------------- | ---------------------------- |
| 1    | Load disk image            | Autopsy / FTK Imager        | Partition & unallocated view |
| 2    | Identify unallocated space | Autopsy File System View    | Sector ranges                |
| 3    | Data carving               | Autopsy Data Carving Module | Recovered files              |
| 4    | Export evidence            | Autopsy Export Option       | File copies for analysis     |


## OUTPUT:
Unallocated Space Analysis and Extracted Data Report
<img width="670" height="387" alt="d1" src="https://github.com/user-attachments/assets/9db83db2-331a-4c06-bfe5-b8bb558808af" />
<img width="1707" height="900" alt="d2" src="https://github.com/user-attachments/assets/6247bd8c-b7a9-4abb-ba9e-06e1f2adf1c9" />
<img width="1711" height="907" alt="d5" src="https://github.com/user-attachments/assets/7ba429c9-99b2-4022-8c8d-e189d525b255" />
<img width="1701" height="901" alt="d6" src="https://github.com/user-attachments/assets/75a8d1b0-b36f-4ca3-9d27-e44f324e23de" />
<img width="1703" height="901" alt="d7" src="https://github.com/user-attachments/assets/ef863b22-d3a7-4317-b5b0-03b424a9be0b" />
<img width="1672" height="941" alt="d12" src="https://github.com/user-attachments/assets/3725c14a-7173-49b8-a9ed-5797e75e879c" />
<img width="1672" height="941" alt="d11" src="https://github.com/user-attachments/assets/a80b344e-c0f3-41b0-ab18-97c6e77c31dd" />







## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

