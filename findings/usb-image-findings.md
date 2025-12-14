# USB Image Analysis

## 1. Summary of Findings
The USB forensic image contains critical evidence linking Roger to an
encrypted and hidden communication channel orchestrated by the
mastermind, identified as Viktor.

The analysis strongly indicates that:
- The USB device was used as a covert communication channel.
- Messages and images of the hostage were concealed within PDF files
  using steganography to maintain secrecy.
- Roger’s actions were performed under direct threat from Jimmy’s
  kidnapper.
- Files were deleted, hidden, and stored in unallocated space to avoid
  detection.

---

## 2. Detailed Analysis

### 2.1 File System Overview
The USB device contained multiple directories and artifacts of forensic
interest, including:
- **$OrphanFile** – Deleted or partially recovered files
- **$UnAlloc** – Unallocated cluster data
- **Jimmy** – Folder containing hostage images
- **Unallocated PDFs** – Deleted PDF files containing hidden data

The majority of PDF files were recovered from unallocated space,
indicating intentional deletion to maintain secrecy.

---

### 2.2 Ransom Note (Key Evidence)
A text file recovered from unallocated space contained the following
message:

> “Repayment for Jimmy.  
> Owed: 250k  
> The deal: transfer the money by Friday or accept the deal to deliver  
> three luxury cars. Confirm your choice by Friday 21/02/2025 to  
> Jimmy’s number. Photos must be hidden using steghide.  
> We have Jimmy, so either pay us back or accept the deal if you want  
> to see him again.”

#### Interpretation of the Ransom Note
The ransom note confirms:
- Jimmy was kidnapped and held hostage.
- Roger was forced to steal luxury cars as an alternative to a cash
  ransom.
- Steganography was explicitly instructed as a method of concealed
  communication.
- Direct threats were made against Jimmy’s life, establishing coercion.

---

### 2.3 Hidden / Steganographic Files
In-depth inspection of the USB image revealed several files labeled as
invoices, including:
- `Invoice_1935.pdf`
- `Invoice_2448.pdf`
- `Invoice_2078.pdf`
- `Invoice_4492.pdf`
- `Invoice_8166.pdf`
- `Invoice_8978.pdf`

#### Metadata Observations
- **MIME Type:** `application/octet-stream` (not a valid PDF)
- **File Size:** Approximately 6 KB, inconsistent with genuine invoice
  documents
- **Location:** Many files recovered from unallocated space
- **Filename Pattern:** Auto-generated short names (e.g., `_NVOIC~3.pdf`)

These characteristics strongly indicate deliberate data concealment
using steganography.

---

### 2.4 Hostage Images
The directory named **Jimmy** contained disturbing images depicting:
- A young male identified as Jimmy
- Blindfolded and restrained conditions
- Visible injuries, including blood around the mouth

#### Interpretation
These images:
- Serve as proof-of-life evidence
- Correlate directly with ransom note instructions regarding hidden
  images
- Confirm the kidnapping of Jimmy
- Explain the coercive pressure that led Roger to participate in the
  car thefts

---

## 3. Conclusion
The USB storage device provides substantial evidence of:
- Criminal coercion through kidnapping
- Hidden communication via steganography
- Explicit ransom instructions
- Hostage documentation used for intimidation

The USB image establishes a foundational component of the case. The
evidence strongly supports the conclusion that Roger’s participation in
luxury car thefts was not voluntary but was carried out under duress due
to the kidnapping of his brother, Jimmy.

