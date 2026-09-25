# Sparx Reader Completer

![Language](https://img.shields.io/badge/Language-C%2B%2B-blue)
![Platform](https://img.shields.io/badge/Platform-Windows-0078D6)
![AI](https://img.shields.io/badge/AI-Google%20Gemini-4285F4)
![Status](https://img.shields.io/badge/Status-In%20Development-orange)
![Release](https://img.shields.io/badge/Release-TBD-lightgrey)

A Windows application written in C++ that automates interactions with Sparx Reader and uses Google's Gemini API to process questions.

## Overview

Sparx Reader Completer is designed to sign in to a Sparx Reader account, open the assigned book, and automatically answer questions using AI. Rather than proceeding immediately, it estimates reading time from the word count and an average reading speed (WPM).

**Note:** Estimated reading delays do not mean that a book has actually been read. Using automation for assigned schoolwork may violate school or platform rules.

## Features

- **Account sign-in:** Prompts for your school, username, and password.
- **Book navigation:** Opens the book associated with your account.
- **AI-powered answers:** Sends question text to Google Gemini for processing.
- **Reading-time estimation:** Calculates delays using word count and average WPM.
- **Windows application:** Built in C++ for distribution as a Windows `.exe`.

## Requirements

- Windows
- A Sparx Reader account
- Your own Google Gemini API key
- An internet connection for Sparx Reader and Gemini API requests

### Google AI API key

The application asks you to enter your own Google Gemini API key. Google offers a **free API tier** for supported models, subject to eligibility and rate limits; paid usage may also be available. Check Google's current [Gemini API billing information](https://ai.google.dev/gemini-api/docs/billing) and [pricing](https://ai.google.dev/gemini-api/docs/pricing) before enabling billing.

Keep your API key private. Do not post it publicly or include it in bug reports. An API key is used to authenticate requests to Google, so it is sent to Google's API along with each AI request.

## Privacy and data handling

The intended data flow is:

| Information | Where it goes |
| --- | --- |
| School, username, and password | Used to sign in directly to Sparx Reader; **not sent to Google AI or the project's developer** |
| Question text | Sent to Google's Gemini API so the AI can process the questions |
| Google Gemini API key | Sent to Google as required to authenticate Gemini API requests |
| Word count and estimated reading delay | Calculated locally by the application |

**Important:** Signing into Sparx Reader requires network communication with Sparx Reader itself. Therefore, it would be inaccurate to say that credentials *never leave your machine*. The intended privacy guarantee is that your school login information is **not forwarded to Google AI or developer-operated servers**.

According to the project's intended design, **question text is the only educational content sent to Google AI**. Actual data handling should be verified before release. Google's free API tier may use submitted content to improve its products; review [Google's current pricing and data-use terms](https://ai.google.dev/gemini-api/docs/pricing) if privacy is important to you.

## Technology

| Component | Details |
| --- | --- |
| Language | C++ |
| Platform | Windows |
| AI service | Google Gemini API (user-supplied key) |
| Distribution | Planned `.exe` |
| Source availability | To be decided |

## Project status

The project is in development. Release format, installation instructions, and source-code availability will be confirmed later.

## Disclaimer

This is an independent project and is not affiliated with or endorsed by Sparx Reader or Google. Users are responsible for following applicable school, platform, and API terms.
