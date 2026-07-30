# Project Case Study: Web Archiving & Capturing Grassroots Ephemera

## Overview

This project explores the preservation of born-digital community records through web archiving workflows. It focuses on capturing ephemeral online materials, including event announcements, social media content, digital publications, and web-based resources that are vulnerable to disappearance due to link rot, platform changes, organizational transitions, or limited digital infrastructure.

Grassroots organizations, community groups, and independent creators increasingly rely on digital platforms as primary spaces for communication, organizing, and historical documentation. These materials often provide valuable evidence of community life but may not be preserved through traditional archival workflows.

---

## Objectives

This case study demonstrates practical approaches for:

* Appraising and selecting born-digital materials for preservation
* Capturing web-based resources using web archiving tools
* Preserving digital ephemera and community documentation
* Creating descriptive metadata and preservation documentation
* Generating fixity information through checksum verification
* Validating archived resources through replay testing
* Addressing rights, ethics, and access considerations in web archiving

---

## Tools & Standards Used

* **Capture Tools:** ArchiveWeb.page / Webrecorder tools
* **Preservation Format:** WARC (Web ARChive) file format, ISO 28500:2017
* **Replay Tool:** ReplayWeb.page
* **Metadata & Documentation:** CSV metadata records, Markdown documentation, preservation notes
* **Fixity Verification:** SHA-256 checksums

---

## Web Archiving Workflow

Each web archiving project follows a documented preservation workflow:

### 1. Appraisal & Selection

Materials are evaluated according to collection scope, archival value, community relevance, and preservation risk. Selection decisions are documented through appraisal records.

### 2. Seed Definition

Target URLs are identified and documented. Capture boundaries are established based on the nature of the resource, platform behavior, and preservation goals.

### 3. Web Capture

Web resources are captured using web archiving tools designed to preserve webpage structure, embedded resources, metadata, and associated digital content when possible.

### 4. WARC Preservation

Captured resources are exported as WARC files, preserving web content, HTTP metadata, timestamps, and associated resources according to the WARC standard.

### 5. Metadata & Documentation

Each preserved item receives descriptive and administrative metadata documenting creator, format, original URL, dates, location, appraisal decisions, and preservation notes.

### 6. Fixity & Validation

Preserved files receive SHA-256 checksums to document file integrity. WARC files are replayed in ReplayWeb.page to verify successful loading and document preservation outcomes and limitations.

---

## Case Studies

### San Diego Lesbian Community Digital Records, Spring–Summer 2026

A born-digital preservation project documenting publicly accessible digital records related to contemporary lesbian community life in San Diego, California. Materials include event webpages, social media content, digital publications, and promotional ephemera preserved through web capture and file-level preservation workflows.

[View Case Study →](./san-diego-lesbian-community-digital-records/)

---

## Archival Reflection

Web archiving has become an essential component of contemporary archival practice. Community histories are increasingly created, shared, and maintained through digital platforms, yet these records remain vulnerable to technological change, platform dependency, and loss.

Preserving grassroots digital materials requires both technical knowledge and archival judgment: determining what should be collected, how it should be captured, what contextual information must be preserved, and how access can be provided while respecting creator rights and community context.
