# CVE-2023-38831 PoC (Proof Of Concept)

This is an easy to use exploit for CVE-2023-38831, a vulnerability that affects WinRAR versions before 6.23.

> An exploitable vulnerability has been identified in RARLabs WinRAR versions prior to 6.23. This vulnerability enables attackers to execute arbitrary code through a specifically crafted ZIP archive. The vulnerability arises due to the mishandling of ZIP archives containing benign files, such as ordinary .PDF document, alongside folders sharing the same name. When a user attempts to access the benign file, the archive may include a similarly named folder containing executable content. This malicious content within the folder is processed during the attempt to access the benign file, facilitating the execution of arbitrary code. The exploitation of this vulnerability has been documented in real-world incidents occurring from April to August 2023

![](assets//image.png)
![](assets/demo_.gif)

# Usage

```bash
git clone https://github.com/HDCE-inc/CVE-2023-38831
cd CVE-2023-38831
python exploit.py
```

# Reference

https://hdce.medium.com/cve-2023-38831-winrar-zero-day-poses-new-risks-for-traders-684911befad2

https://www.group-ib.com/blog/cve-2023-38831-winrar-zero-day/
