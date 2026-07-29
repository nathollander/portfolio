# Digital Preservation Workflow: BagIt Packaging for Digitized LGBTQ+ Archival Materials

## Project Overview

This project demonstrates a digital preservation workflow for publicly accessible digitized archival materials from the **Lydia R. Otero Archive at Los Angeles Public Library Special Collections**.

You can explore the project directory structure, metadata, and files directly in the [Lydia Otero BagIt Project folder](https://github.com/nathollander/lydia-otero-bagit-preservation-workflow/tree/main/Lydia_Otero_Bagit_Project%20copy). Payload files have been omitted for demonstration purposes, due to repository rights restrictions. Original files were accessed through the Los Angeles Public Library digital collections platform.

Using the Library of Congress BagIt File Packaging Format, this workflow establishes a standardized preservation package, creates SHA-256 fixity information, and validates the integrity of digitized archival objects.

The purpose of this project was to demonstrate practical application of digital preservation concepts including:

- preservation packaging
- cryptographic checksums
- fixity verification
- provenance documentation
- ethical use of archival digital objects

---

# Source Collection

**Repository:** Los Angeles Public Library Special Collections

**Collection:** Lydia R. Otero Archive

**Selected Materials:** Digitized ephemera created by Lesbianas Unidas of Gay and Lesbian Latinos Unidos documenting Latina lesbian community organizing, fundraising activities, and conference events.

Selected digital objects include:

- Fundraiser for Lesbianas Unidas at Robbie's Disco (1987)
- Festejemos una noche de baile Latina
- 1st annual Hair Cut-A-Thon (1987)
- First National Latina Lesbian Conference

The original digital objects were accessed through the Los Angeles Public Library digital collections platform.

---

# Tools & Standards

## Specification

**BagIt File Packaging Format (RFC 8493)**

BagIt is a hierarchical file packaging format used to organize digital content and associated metadata for reliable transfer and storage.

## Software

**Library of Congress Bagger**

Used to create and validate the BagIt preservation package.

## Fixity Algorithm

**SHA-256 Cryptographic Checksum**

SHA-256 hashes provide a unique digital fingerprint for each payload file. These checksums allow archivists to detect unintended changes to files after transfer or storage.

---

# Preservation Workflow

## 1. Metadata Capture

Repository-provided descriptive metadata was recorded before packaging, including:

- repository identifiers
- titles
- creators
- dates
- collection information
- rights information

## 2. File Acquisition

Four digitized archival objects were downloaded from the Los Angeles Public Library digital collections platform.

## 3. BagIt Creation

The files were packaged using Library of Congress Bagger according to the BagIt specification.

The resulting package included:

```text
lydia_otero_digital_preservation_demo/
├── bagit.txt
├── bag-info.txt
├── manifest-sha256.txt
├── tagmanifest-sha256.txt
└── data/
    ├── archives_15.jpg
    ├── archives_21.jpg
    ├── archives_22.jpg
    └── archives_183.jpg
```

## 4. Fixity Generation

SHA-256 checksums were generated for each payload file and recorded in the preservation manifest.

## 5. Validation

The completed BagIt package was validated to confirm that all payload files matched their recorded checksums.

---

# Validation Results

## Successful Validation

The completed preservation package successfully passed BagIt validation.

Result: PASS


## Controlled Fixity Test

A copy of the validated BagIt package was intentionally modified by altering one payload file.

The modified package was validated again.

Result: FAIL


The validation failure demonstrated that SHA-256 fixity checks can identify unauthorized changes to preserved files.

---

# Rights & Ethical Considerations

The selected materials remain subject to the rights and reproduction restrictions established by the Los Angeles Public Library.

This project uses publicly accessible digitized archival materials for educational and research purposes. Original digital objects are not redistributed through this repository.

Documentation and metadata are provided to demonstrate preservation workflow practices while respecting repository access policies.

---

# Preservation Reflection

This project demonstrates how standardized preservation workflows can support responsible stewardship of community archival materials.

While BagIt does not preserve the historical meaning of records by itself, it provides essential technical infrastructure by documenting file integrity, supporting reliable transfer, and enabling future verification across storage environments.

For community archives and smaller collecting organizations, accessible preservation tools such as BagIt provide practical methods for strengthening long-term digital stewardship.

---

# Repository Contents
```text
├── documentation/
│   ├── provenance.md
│   ├── workflow.md
│   └── validation_report.md
│
├── metadata/
│   └── lydia_otero_inventory.xlsx
│
├── screenshots/
│   ├── validation_success.png
│   └── fixity_test_failure.png
│
└── sample_structure/
    └── bag_structure.txt
```
