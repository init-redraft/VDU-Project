# VDU App: Veteran Discharge Upgrade Locator

## Intro
If a veteran is discharged and they feel that the discharge type, classification or other information was unfairly assigned or handled. There is a convoluted and opague process to submitted a request to the DOD to have the file reviewed and your discharge upgraded or amended. Once a veteran has gathered the necessary information and submitted it to the appropriate party, it goes into a silent process that can more than a year in to even receive a response. This leaves many veterans haunting the halls of the ARBA Reading Rooms, if they even know about this resource, in hopes of finding a sudden snippet of infomration on whether their request was approved.

This causes anxiety and an emotional toll. To aid in this, I am building a simple web app that will utilize publicly available open source information to provide veterans with case status updates when the ARBA Reading Room publishes their case file. 

Modular Python tool designed to locate and parse discharge upgrade files across .MIL and VA portals.

> **Note:** This tool is designed to help veterans reduce their need to constantly stalk the .MIL reading rooms. Also designed with a focus on enabling visibility for veterans and VSOs. Built as part of a portfolio as I develop skills across Cyber Security domains.

## Features
- Static URL Parsing for known upgrade portals.
- Modular file locator with extensible architecture.
- Ethical design: no scraping, impersonation or unauthorized access. 

> **Note:** All features are designed compliance and ethical rigor in mind. Future phases include PDF delivery and dashboard integration. 

## Planned Phases
1. Single case query handling.
    []Complete `file_locator.py`
    []Complete `main.py`
    []Complete `requirements.txt`
    []Establish tool hosting
    []Test tool thoroughly using known good information
    []Publish tool and share to known veteran groups and local VSOs
2. PDF download and metadata validation.
    []Scaffold next iteration structure
    []Create PDF hanlding .py
    []Ensure secure handling of file with no data retention
3. Email Alerting for individual veterans and VSO case managers. 
    []Scoffold next iteration structure
    []Create email sign up form, database and alert handling to align with best practices and mitigate scraping
    []Test thoroughly
    []Ensure secure handling of PII.
4. Web dashboard for multiple file status tracking for VSO case managers. 
    []Scaffold next iteration structure
    []Build out UI/UX for VSO Dashboard
    []Structure backend to allow for single users to track multiple cases with clear identifiers of which cases have sourced files available and which do not.
    []Idenitify and implement access controls to ensure only authorized VSOs are utilizing. 
    []Test thoroughly

**Note:** Each phase is modular and independently deployable. Designed to support phased Github commits.

## Disclaimer
This tool does not store or transmit PII or any other sensitive information. This tool is intended for use by veterans and VSOs to monitor and review any changes to their case files and case file status. This tool is entirely developed by me and is not sponsored or affilliated with the DOD, VA, any branch of the military or any department in the government.