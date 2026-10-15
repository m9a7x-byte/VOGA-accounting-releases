# VOGA Accounting Releases

Official Windows x64 installers for VOGA Accounting by ABBAS IT.

This repository contains release artifacts only. Application source, customer databases, attachments, activation private keys and signing private keys are not uploaded here.

## Installation

Download the installer from Releases. A permanent license bound to one computer is required. Send the activation request displayed by the application to the publisher and import the issued `.vogalicense` file. Updates do not remove an existing activation or local SQLite data.

Installers are self-signed by ABBAS IT. Self-signing does not provide automatic Windows trust or guarantee the absence of SmartScreen warnings. The application separately verifies update releases using an embedded Ed25519 public key and SHA-512 before installation. The `.cer` release asset is public certificate information, not a private key; importing it into Windows trust is not required for the application's update verification.

## Updates

The installed application checks GitHub for stable releases. The system administrator chooses when to download and install. The application saves a local database/attachment backup before installation. Business data remains local and is not uploaded to GitHub.

`latest.yml`, the installer blockmap, and `release-integrity.json` are consumed by the update client. Do not edit or replace published assets in place. Publish a newer version instead.
