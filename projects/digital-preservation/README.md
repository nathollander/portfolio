# Project Case Study: Digital Preservation & Ingest using BagIt

## Objective
To establish a verifiable, secure chain of custody and baseline fixity for digital-born community materials upon ingest into an archival repository.

## Tools & Standards Used
* **Specification:** Library of Congress BagIt File Packaging Format (RFC 8493)
* **Software:** Library of Congress Bagger GUI tool
* **Algorithm:** SHA-256 Cryptographic Checksum

## The Scenario
A local grassroots organizer donates a collection of digital files containing minutes, posters, and flyers from local pride organizing committees from 2005 to 2010. To prevent silent file corruption ("bit rot") and prove the files were not altered during transfer, the assets must be packaged into a standardized directory structure called a "bag."

---

## The Structural Architecture of the "Bag"

Below is the file directory structure generated for this collection. The `data/` directory holds the original payload, while the root text files serve as the preservation manifests.

```text
pride-committee-collection/
├── bagit.txt                 # Declares the BagIt version and encoding character set (UTF-8)
├── bag-info.txt              # Administrative metadata (Donor info, contact, bag date, size)
├── manifest-sha256.txt       # The critical preservation file containing checksums for all data files
├── tagmanifest-sha256.txt    # Verifies the integrity of the manifest files themselves
└── data/                     # THE PAYLOAD (Untouched original archival assets)
    ├── minutes_2005.pdf
    ├── minutes_2006.pdf
    ├── pride_poster_2007.jpg
    └── outreach_flyer_2010.png
```

### The Manifest File (`manifest-sha256.txt`)
Inside the manifest, every file in the payload is assigned a unique cryptographic fingerprint. If even a single letter in a PDF is changed, the checksum breaks, alerting the archivist to file corruption:

```text
5e884898da28047151d0e56f8dc6292773603d0d6aabbdd62a11ef721d1542d8  data/minutes_2005.pdf
a1b2c3d4e5f61234567890abcdef1234567890abcdef1234567890abcdef1234  data/minutes_2006.pdf
f823bc891a27de45f8cde01a23bcde45f6789ab01234cd5678ef0123456789ab  data/pride_poster_2007.jpg
```

---

## 💡 Archival Reflection
Independent, community-run organizations often lack the enterprise servers of major academic libraries. Implementing a standard tool like BagIt allows small archives to verify file integrity on standard desktop computers. Running regular fixity checks against these SHA-256 manifests guarantees that community history remains completely uncorrupted over generations of server migrations.
