
# Windows Image Forensic Analysis

## 1. Overview
The Windows forensic image was analyzed using **Autopsy** to identify user
activity, communication methods, and file-based artifacts relevant to the
investigation. The analysis focused on installed tools, browsing activity,
email access, and unusual file-naming patterns.

---

## 2. User Account Attribution
Artifacts recovered during the analysis were attributed to the following
user account:

- **Username:** Roger

The majority of evidence was consistently located under:

This confirms that the artifacts identified during the analysis are
directly attributable to the suspect.

---

## 3. Steganography Tool Presence
### Discovery of `steghide.exe`
A steganography tool, **steghide**, was identified on the Windows system.

- **File Name:** `steghide.exe`
- **Location:**  
  `C:\Users\roger\Downloads\steghide-0.5.1-win32\steghide\`

The executable was present as an allocated file. A corresponding
**Zone.Identifier** alternate data stream was also identified, confirming
that the file was downloaded from the internet.

#### Interpretation
The presence of `steghide.exe` indicates that the suspect had access to a
tool capable of hiding data within other files. While direct evidence of
execution was not identified, its presence aligns with the steganographic
artifacts discovered on the USB device.

---

## 4. Use of Online File Conversion Tools
### Evidence of Web-Based File Processing
Analysis of web download artifacts revealed the use of an online file
conversion service.

#### Findings
- The service **freeconvert.com** was accessed.
- Multiple files were downloaded from this service.
- **Zone.Identifier** metadata confirmed the files originated from the
  internet.

#### Interpretation
The suspect appears to have used online conversion services instead of
locally installed software, likely to minimize the forensic footprint on
the system.

---

## 5. Unusual File Naming Patterns
Analysis revealed a password-protected archive named **`food.zip`**. The
archive had also been extracted, revealing files with unconventional
naming conventions.

### Numerically Named Files
The extracted folder contained image files with purely numeric names
(e.g., `1.jpg`, `2.jpg`). These files were valid images and depicted luxury
vehicles.

### Decimal-Named Files
Another set of image files used decimal-based numeric names
(e.g., `1.1.jpg`, `2.2.jpg`). These files contained images of food.

#### Interpretation
This pattern suggests deliberate obfuscation, where images of luxury cars
were concealed among benign food images. The structure may have been used
to communicate or select target vehicles while avoiding immediate
detection.

---

## 6. Email Communication Evidence

### 6.1 Gmail Web Access
Keyword searches for **`mail.google.com`** revealed extensive browser cache
and network artifacts.

#### Findings
- Gmail-related artifacts were located under:
  - `AppData\Local\Google\Chrome\User Data\Default\`
  - `AppData\Local\Microsoft\Edge\User Data\Default\`
- Cache files, cookies, and network state files were identified.
- Multiple timestamps indicated repeated access to Gmail.

---

### 6.2 Microsoft Outlook Web Access
Additional keyword searches for **`outlook`** and **`outlook.office.com`**
revealed further web-based email artifacts.

#### Findings
- Outlook web interface artifacts were identified.
- Calendar-related strings and web components were present.
- No Outlook desktop mail database files were found.

#### Interpretation
The absence of local email databases indicates the use of **web-based email
services**, where message content is stored remotely rather than on the
local system, supporting intentional secrecy.

---

## 7. Summary of Findings
The following key observations were established from the Windows image
analysis:
- The user account **Roger** was actively used.
- A steganography tool (`steghide.exe`) was present on the system.
- Online file conversion services were utilized.
- Luxury car images were deliberately hidden among food images.
- Repeated access to web-based email services such as Gmail and Outlook
  was identified.

---

## 8. Conclusion
The Windows image analysis indicates that the suspect relied heavily on
web-based tools and services, including browser-based email platforms, to
avoid storing sensitive communication locally.

Additionally, deliberate file-handling behavior was observed through the
presence of steganography tools and unconventional file-naming practices.
These findings align with the broader evidence of concealed communication
and coercion identified across the phone and USB forensic images.

