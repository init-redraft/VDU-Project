# VDU App Architecture

## Overview
The app uses modular Python scripts to locate discharge upgrade files across known .MIL and VA portals.

**Note:** Architecture avoids scraping by relying on static URLs and user-initiated queries. Designed to remain complaint with federal data access norms.

## Module Breakdown
- `file_locator.py` : parses known portal structures and flags upgrade related documents. 
- `pdf_handler.py` : (planned): extracts and validates metadata from downloaded PDFs.
- `email_alert.py` : (planned): Sends alerts to individual veterans or VSOs based on file status.

> **Note:** Each module is compartmentalized to support phased deployment and Github versioning. Future models will be added as seperate branches.

## Security Considerations
- No Credential storage or impersonation
- All access is read-only and user-intitiated
- Logs are local and non-persistent

> **Note:** Security boundaries are modeled to align with ethical standards and avoiding triggering compiance flags.