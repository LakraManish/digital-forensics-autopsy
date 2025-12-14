# Forensic Methodology

## Investigation Approach
This investigation followed a structured and repeatable digital forensic
methodology to ensure evidence integrity, accuracy, and proper
interpretation.

The analysis was conducted on three forensic images:
- Windows 11 system image
- Android mobile phone image
- USB storage device image

All examinations were performed in a read-only manner to preserve the
original evidence.

---

## Tools Used
- **Autopsy 4.22.1** – Digital Forensics and Incident Response (DFIR)
- Built-in Autopsy ingest modules:
  - Keyword Search
  - File Metadata Analysis
  - Timeline Analysis
  - Deleted File Recovery
  - Web Artifacts Analysis

---

## Examination Process

### 1. Evidence Ingestion
Each forensic image was added to Autopsy as a separate data source. Only
relevant ingest modules were enabled based on the image type to optimize
analysis time and accuracy.

### 2. Artifact Identification
Key artifacts were identified, including:
- SMS and messaging data
- Discord cache files
- Browser history, cache, and cookies
- Email web access artifacts
- Encrypted and steganographic files
- Deleted and unallocated data

### 3. Correlation Across Devices
Findings from the phone, USB, and Windows images were correlated to
identify relationships between events, communication methods, and file
usage across multiple platforms.

### 4. Timeline Reconstruction
Autopsy’s timeline feature was used to reconstruct the sequence of
events, helping to understand the progression from kidnapping to
coerced criminal activity.

### 5. Interpretation and Reporting
All findings were analyzed objectively. Conclusions were drawn only
where supported by multiple artifacts or corroborating evidence.
