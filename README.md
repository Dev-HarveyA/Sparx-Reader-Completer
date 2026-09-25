# Sparx Reader Completer

![Language](https://img.shields.io/badge/Language-C%2B%2B-blue)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6)
![Status](https://img.shields.io/badge/Status-In%20Development-orange)
![Release](https://img.shields.io/badge/Release-TBD-lightgrey)

A Windows application written in C++ that automates interactions with Sparx Reader.

## Overview

Sparx Reader Completer is designed to sign in to a Sparx Reader account, open the assigned book and automate answering questions. It calculates a delay based on the amount of text and an average words-per-minute (WPM) reading speed rather than progressing immediately.

**Note:** Automated timing is not evidence that a book has actually been read. Using automation for assigned schoolwork may violate school or platform rules.

## Features

- **Account sign-in:** Prompts for a school, username and password.
- **Book navigation:** Opens the book associated with the account.
- **Automated question answering:** Processes questions as part of the automated workflow.
- **Reading-time estimation:** Uses word count and average WPM to calculate delays.
- **Windows application:** Developed in C++ for distribution as a Windows `.exe`.

## Technology

| Component | Details |
| --- | --- |
| Language | C++ |
| Platform | Windows |
| Distribution | Planned `.exe` |
| Source availability | To be decided |

## Project status

The release format, installation instructions and source-code availability have not yet been finalized. This README will be updated when those details are confirmed.

## Security and privacy

The application requests Sparx Reader login credentials. Before releasing it, document how credentials are handled and ensure that passwords are not logged or stored insecurely. Users should understand what information the application accesses.

## Disclaimer

This is an independent project and is not affiliated with or endorsed by Sparx Reader. Users are responsible for following applicable school and platform rules.
