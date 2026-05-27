# pcip-fhir-callback

Public static site for the **PCIP (Personal Cancer Intelligence Platform)** Epic & Athenahealth FHIR app registration.

## Purpose

SMART-on-FHIR / OAuth 2.0 app registration with Epic and Athenahealth requires a publicly reachable:
- **OAuth redirect / callback URL**
- **Terms of service page**

This repository serves those static pages. It contains **no PHI, no credentials, and no application logic** — only the minimal public-facing pages the FHIR app registration process requires.

## Contents

- `index.html` — OAuth callback landing page
- `terms.html` — terms of service
- `pcip-logo.png` — logo

## Related repository

The actual Personal Cancer Intelligence Platform — clinical data, analysis, build tooling, and the FHIR integration / MCP server code — lives in the **private** `pcip` repository. This repo is intentionally public and minimal; the platform repo is private because it contains protected health information (PHI).

| Repo | Visibility | Purpose |
|------|-----------|---------|
| **pcip-fhir-callback** (this repo) | Public | Static OAuth callback + terms pages for FHIR app registration |
| **pcip** | Private | The platform: clinical data, analysis, build tooling, integration/MCP code |
