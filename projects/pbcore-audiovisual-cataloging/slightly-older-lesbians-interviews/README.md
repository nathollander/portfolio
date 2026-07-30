# Women's Interviews for Slightly Older Lesbians — PBCore Audiovisual Cataloging Case Study

## Overview

This case study demonstrates the application of PBCore metadata standards to a digitized audiovisual archival object. The selected record, *Women's interviews for Slightly Older Lesbians*, documents interviews conducted with members of Slightly Older Lesbians, a San Diego-based lesbian social organization.

The original audiovisual material was preserved as a 1/2 inch videotape held by Lambda Archives of San Diego and made publicly accessible through California Revealed. This project creates a structured audiovisual metadata record documenting the relationship between the original physical carrier and its digital derivative.

---

## Project Objectives

This case study demonstrates workflows for:

- Applying PBCore metadata standards to audiovisual materials
- Mapping descriptive, technical, and preservation metadata
- Documenting relationships between physical carriers and digital derivatives
- Characterizing audiovisual file properties using technical metadata tools
- Recording preservation considerations for digitized moving image collections

---

## Source Object

**Title:**  
Women's interviews for Slightly Older Lesbians

**Repository:**  
Lambda Archives of San Diego

**Original Format:**  
1/2 inch videotape

**Digital Derivative:**  
MP4 access copy

**Date Created:**  
July 20, 1991

**Duration:**  
23 minutes, 13 seconds

---

## Metadata & Preservation Workflow

The workflow included:

1. Review of the repository record and existing descriptive metadata
2. Creation of a PBCore XML record describing the audiovisual object
3. Identification of contributors, subjects, coverage, rights information, and instantiation details
4. Download and verification of the digital access copy
5. SHA-256 checksum generation for file integrity verification
6. Technical characterization using FFprobe
7. Documentation of preservation considerations and digital object relationships

---

## Tools & Standards Used

**Metadata Standard**
- PBCore 2.1

**Controlled Vocabulary**
- Homosaurus
- Locally developed descriptive terms

**Technical Characterization**
- FFprobe (FFmpeg)

**Fixity Verification**
- SHA-256 checksum

**File Format**
- MP4 container
- H.264 video
- AAC audio

---

## Repository Structure
```text
pbcore-audiovisual-cataloging/
└── slightly-older-lesbians-interviews/
    ├── README.md
    ├── source-metadata/
    │   └── source-record.md
    ├── documentation/
    │   ├── pbcore-mapping.md
    │   ├── technical-metadata.md
    │   └── preservation-notes.md
    └── pbcore/
        └── slightly-older-lesbians-interviews.xml
```



---

## Rights & Access

The original audiovisual material remains subject to the rights, restrictions, and access policies established by Lambda Archives of San Diego.

This project is an independent metadata and preservation documentation exercise using publicly accessible archival materials. The resulting PBCore record does not replace or modify the repository's official catalog record.

---

## Archival Significance

Audiovisual community records document experiences, activism, and cultural histories that may otherwise remain inaccessible or underrepresented. Structured metadata supports improved discovery, preservation planning, and long-term stewardship of moving image collections.

