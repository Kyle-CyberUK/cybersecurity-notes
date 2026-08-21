# Digital Forensics

## Overview
- Introduces how digital evidence is collected, examined, and analysed following a cybercrime.
- It covers the NIST forensics methodology, types of digital forensics, evidence acquisition best practices, and Windows forensics tools.

## Key Concepts
- **Digital Forensics** is the branch of forensics that investigates cybercrime; any crime conducted on or using a digital device.

## NIST Forensics Methodology (4 phases)
- **Collection** - Identify and securely gather evidence without tampering.
- **Examination** - Filter and extract only the relevant data.
- **Analysis** - Correlate evidence to draw accurate conclusions.
- **Reporting** - Produce a detailed report of methodology and findings.

## Types of Digital Forensics
- **Computer** - Desktops, laptops — most common devices.
- **Mobile** - Call records, messages, GPS data.
- **Network** - Traffic logs across the whole network.
- **Database** - Intrusions resulting in data modification or exfiltration.
- **Cloud** - Evidence stored on cloud infrastructure — can be tricky as little evidence on the cloud.
- **Email** - Phishing and fraudulent email campaigns.

## Evidence Acquisition
- **Proper Authorisation** - Evidence collected without approval may be inadmissible in court.
- **Chain of Custody** - A formal document logging who collected evidence, when, where it's stored, and who has accessed it.
- **Write Blockers** - Hardware that prevents any alteration to the original evidence during collection.

## Windows Forensics Tools
- **FTK Imager** - Disk image acquisition and analysis.
- **Autopsy** - Open-source platform for analysing disk images.
- **DumpIt** - Memory image acquisition via CLI.
- **Volatility** - Open-source memory image analysis.
- Two image types are collected from Windows systems:
  - **Disk Image** - non-volatile data (files, browsing history, documents)
  - **Memory Image** - volatile data (running processes, open files, network connections) — must be taken first before shutdown.

## Forensics Tools - Practical
- `pdfinfo` - reads metadata from PDF files (author, creator, creation date):
  - `pdfinfo document.pdf`
- `exiftool` - reads EXIF metadata from images (camera model, GPS coordinates, timestamps):
  - `exiftool image.jpg`
  - GPS coordinates embedded in photos can reveal where an image was taken.

## Relevance
- Digital forensics is a core blue team discipline and directly supports SOC and incident response work.
- Understanding how evidence is collected and analysed is essential for investigating breaches, supporting legal proceedings, and working in roles such as an SOC Analyst.
