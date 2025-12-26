# Acme-Client-Security-Hash-
UiPath RPA project using ACME System 1 to generate Client Security Hashes with a Dispatcher/Performer architecture. The Dispatcher extracts and queues client data, while the Performer generates and submits SHA1 hashes. Built with best practices, robust error handling, logging, retries, and Orchestrator queues for scalability.
ACME – Client Security Hash (UiPath RPA)
Overview

This UiPath RPA project automates the ACME System 1 – Client Security Hash process using a Dispatcher / Performer architecture.
The automation securely processes client data, generates a SHA1 hash, and updates ACME work items following UiPath best practices.

Architecture
Dispatcher

Logs into ACME System 1

Extracts client data from Work Items

Filters and validates data

Adds valid transactions to Orchestrator Queue

Performer

Retrieves transactions from the Queue

Generates Client Security Hash (SHA1)

Updates ACME Work Items

Handles business and system exceptions

Key Features

Dispatcher / Performer pattern

Orchestrator Queues

Secure hash generation (SHA1)

Robust error handling

Retry mechanism

Detailed logging

Config-driven (Config.xlsx)

Error Handling

Business Exceptions: Missing or invalid client data

System Exceptions: Application, selector, or network issues

Automatic retries and proper transaction status updates

Best Practices Used

REFramework structure

Configurable settings

Modular workflows

Clear logging and traceability

No hardcoded values

Requirements

UiPath Studio

UiPath Orchestrator

ACME System 1 (Test Environment)

Author

Mohamed Raafat
RPA Developer | UiPath | Automation Enthusiast
