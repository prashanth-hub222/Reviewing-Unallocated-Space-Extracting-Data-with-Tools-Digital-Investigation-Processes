# Reviewing-Unallocated-Space-Extracting-Data-with-Tools-Digital-Investigation-Processes
### NAME -Prashanth Raaj S
### REG NO - 212225100035
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
<img width="1600" height="900" alt="image" src="https://github.com/user-attachments/assets/e2170e00-5be9-4dea-a5dd-ce28d7d3a3c7" />
<img width="1600" height="898" alt="image" src="https://github.com/user-attachments/assets/13ebd048-a30f-4ec1-96e8-1116fb11bdc0" />
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/9e89ba88-2737-4fbe-8d50-7a855094fb1c" />
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/91851f2c-e916-4a81-a27a-e4840f31e29a" />
<img width="1600" height="899" alt="image" src="https://github.com/user-attachments/assets/72f60c9a-190e-42b4-ae19-10d49ceca1ea" />
<img width="1600" height="779" alt="image" src="https://github.com/user-attachments/assets/c2050f97-5d0d-46c7-b383-7c2fbfba5ee6" />
<img width="1600" height="740" alt="image" src="https://github.com/user-attachments/assets/08db9a18-1b5f-4c5b-91c0-4a11ecfbd3ac" />


## RESULT:
The unallocated space was successfully analyzed, data was extracted, and the digital investigation process was followed effectively.

