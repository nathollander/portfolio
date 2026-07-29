# Project Case Study: Audiovisual Cataloging using PBCore

## Objective
To create a structurally sound metadata record for a community-based moving image asset, ensuring its long-term discoverability and digital preservation path.

## Tools & Standards Used
* **Schema:** PBCore 2.1 (Public Broadcasting Metadata Dictionary)
* **Vocabularies:** Homosaurus Vocabulary (v3), Library of Congress Name Authority File (LCNAF)

## The Asset
* **Title:** Oral History Interview with Local LGBTQ+ Activists, 1992
* **Format:** Digitized Betacam SP videotape (now an MP4 file)

---

## The PBCore XML Record
Below is the structural metadata block I constructed to map both the descriptive content and the technical specifications of this video file.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<pbcoreDescriptionDocument xmlns="http://pbcore.org">
  
  <!-- Asset Identification -->
  <pbcoreIdentifier source="Local Archive ID">QA-1992-OH-042</pbcoreIdentifier>
  <pbcoreTitle titleType="正式 (Formal)">Interview with June Mazer and Activists at March on Washington</pbcoreTitle>
  <pbcoreDescription descriptionType="Abstract">An oral history interview discussing lesbian visibility, grassroots organizing in Southern California, and logistics surrounding the 1993 March on Washington.</pbcoreDescription>
  
  <!-- Controlled Vocabularies (Homosaurus) -->
  <pbcoreSubject source="Homosaurus" ref="https://homosaurus.org">Lesbian activism</pbcoreSubject>
  <pbcoreSubject source="Homosaurus" ref="https://homosaurus.org">Grassroots organizing</pbcoreSubject>
  
  <!-- Technical Curation & Instantiation -->
  <pbcoreInstantiation>
    <instantiationIdentifier source="File Name">QA-1992-OH-042_preservation.mp4</instantiationIdentifier>
    <instantiationDigital>video/mp4</instantiationDigital>
    <instantiationLocation>Digital Preservation Repository / Video / 1992/</instantiationLocation>
    <instantiationDuration>00:45:12</instantiationDuration>
    <instantiationFileSize units="GB">2.4</instantiationFileSize>
    <instantiationDataRate units="Mbps">7.2</instantiationDataRate>
  </pbcoreInstantiation>

</pbcoreDescriptionDocument>
```

---

## Archival Reflection
Traditional schemas like Dublin Core lack the fields required to document complex AV media data rates, file sizes, and containers. Implementing PBCore ensures that future digital archivists can monitor the technical stability of this video, while using the Homosaurus guarantees that researchers can locate this specific activist history using respectful, community-approved terms.
