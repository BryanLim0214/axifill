# AIXFil-Detect

**AIXFil-Detect: Post-Hoc Forensic Attribution of Insider Data Exfiltration Through AI Chatbot Interfaces**

Generative AI tools have introduced a data theft pathway that standard security tools cannot see: an employee copies sensitive text from a company file and pastes it into a browser-based chatbot. The file never leaves the computer through a traditional channel, so no firewall or data loss prevention system fires an alert. 

AIXFil-Detect is an open-source forensic tool that reconstructs these events after the fact by combining evidence from five Windows data sources:
- Browser history
- Windows clipboard database
- File access timestamps
- Windows Prefetch execution logs
- Network packet captures

Each group of related events is scored with a Weighted Artifact Correlation Score (WACS) that factors in evidence from each source, whether the clipboard text matches the opened file, how much data was uploaded, and the time of day. 

## Experimental Results
We tested the tool on 30 simulated scenarios and achieved a precision, recall, and F1 score of 1.00 at a WACS threshold of 75 using a 30-second time window.

## Repository Contents
- `aixfil_detect_paper.tex` - LaTeX source for the IEEE Conference Paper.
- `aixfil_detect_paper.pdf` - Compiled PDF.
- `figures/` - Directory containing all evaluation charts and diagrams.
- `aixfil_references.bib` - Bibliography references.

## Authors
- Panhapiseth Lim
- Halimat Popoola
- (Mentorship by Dr. Zulfiqar Khan)

Department of Computer Science & Electrical Engineering
The University of Texas Permian Basin
