# Browser Encryption  (If you want buy u can add me on discord "ibo" or Telegram @SluttyDevs

<p align="center">
 <a href="https://t.me/SluttyDevs">
  <img src="https://img.shields.io/badge/Telegram-%40SluttyDevs-26A5E4?logo=telegram&logoColor=white" alt="Telegram @SluttyDevs">
  </a>
  <img src="https://img.shields.io/badge/Discord-ibo-5865F2?logo=discord&logoColor=white" alt="@ibo">
  <img src="https://img.shields.io/badge/Platform-Windows%20x64-0078D6?logo=windows&logoColor=white" alt="Windows x64">
  <img src="https://img.shields.io/badge/Runtime-Node.js%2018%2B-339933?logo=node.js&logoColor=white" alt="Node.js 18+">
  <img src="https://img.shields.io/badge/Native-C%2B%2B-00599C?logo=cplusplus&logoColor=white" alt="Native C++">
  <img src="https://img.shields.io/badge/Status-Working-success" alt="Still Works Fine">
</p>

<p align="center">
  <strong>Authorized security research into modern browser data-protection mechanisms on Windows.</strong><br>
  <sub>Chromium App-Bound Encryption - Windows DPAPI - Gecko NSS - Native Node.js Integration</sub>
</p>

---

## Overview

This project is a proof-of-concept research module developed to evaluate how modern web browsers protect locally stored authentication data on Windows.

The research covered Chromium- and Gecko-based browsers, multiple browser profiles, legacy DPAPI-protected records, and newer App-Bound Encryption protections. The finding was tested in a controlled environment.

To reduce misuse, this repository intentionally omits operational instructions, sensitive implementation details, extraction procedures, and real authentication data.

## Research Scope

The module was designed to assess:

- **Chromium-based browsers**, including modern App-Bound Encryption behavior.
- **Gecko-based browsers**, including NSS-backed data protection.
- **Multiple local browser profiles** and their encrypted storage formats.
- **Native Windows security boundaries** involved in protecting browser data.
- **Compatibility differences** between legacy and current encryption schemes.

## High-Level Capabilities

During authorized testing, the research prototype demonstrated the ability to:

- Identify supported browser installations and local profiles.
- Distinguish between supported encryption and storage formats.
- Interact with native Windows and browser security components.
- Validate the accessibility and integrity of protected records.
- Process test datasets asynchronously through a Node.js interface.
- Produce controlled research output for verification and reporting.

Specific recovery logic, memory-analysis techniques, internal signatures, cryptographic material, and end-to-end implementation details are intentionally not documented.

## Architecture

```text
JavaScript Interface
        |
Native Node.js Addon
        |
Windows and Browser Security Components
        |
Encrypted Local Browser Storage
        |
Controlled Validation Output


The project combines a JavaScript-facing API with a native implementation. This separation keeps application-level integration straightforward while allowing controlled interaction with operating-system and browser security facilities.

## Technology Overview

| Component | Technology | Role |
|---|---|---|
| Runtime | Node.js | Public module interface and orchestration |
| Native layer | C++ / Node-API | Integration with Windows-native functionality |
| Storage | SQLite | Analysis of browser database structures |
| Cryptography | Windows and browser APIs | Authorized validation of protected records |
| Gecko integration | NSS / PKCS#11 | Compatibility research for Gecko-based browsers |
| Analysis | Native instrumentation | Controlled runtime security research |

## Supported Research Targets

### Chromium family

- Google Chrome
- Microsoft Edge
- Brave
- Opera
- Opera GX

### Gecko family

- Mozilla Firefox
- Waterfox
- LibreWolf
- Floorp
- Zen Browser


## Responsible Disclosure

The underlying security finding followed a coordinated disclosure process:

| Field | Status |
|---|---|
| Research environment | Controlled and authorized |
| Vendor notification | Completed |
| Vendor remediation | Completed |
| Bug bounty recognition | Awarded |
| Sensitive technical details | Withheld |
| Real credentials or session data | Not published |

A redacted vendor acknowledgement, case reference, or bounty confirmation may be included under `docs/` as supporting evidence. Personally identifiable information, authentication data, reusable session material, and confidential vendor correspondence must remain removed.

## Evidence

The following redacted materials can be used to demonstrate the research outcome without exposing sensitive data:

- Vendor acknowledgement or case reference.
- Remediation confirmation.
- Bug bounty award confirmation.
- Sanitized output produced from synthetic test profiles.
- A high-level research timeline.

Raw cookie values, passwords, encryption keys, session tokens, personal profile paths, and live browser databases must not be committed.

## Security and Ethics

This project was created exclusively for:

- Authorized security research.
- Defensive testing in controlled environments.
- Academic study of browser security mechanisms.
- Responsible vulnerability disclosure.
- Validation using owned or synthetic test data.

It must not be used to access another person's device, credentials, accounts, browser profiles, or authenticated sessions. Possession of the code does not constitute authorization.

## Publication Policy

To preserve the defensive value of the research while limiting abuse, the public version does not include:

- Step-by-step reproduction instructions.
- Complete extraction or decryption workflows.
- Runtime locations, signatures, or matching rules.
- Reusable cryptographic material.
- Real passwords, cookies, or session tokens.
- Unsanitized proof-of-concept output.
- Operational examples that enable unauthorized access.

## Project Status

The reported issue has been addressed by the affected vendor. This repository is retained as a portfolio record of the research, native development work, and responsible disclosure process.

It should not be treated as a current exploitation guide, a production credential-recovery tool, or a guarantee of compatibility with present browser releases.

## License

Source code included in this repository is licensed under the terms specified in the `LICENSE` file.

The license does not grant authorization to access systems or data. Users remain responsible for obtaining explicit permission and complying with applicable laws, platform rules, and vendor policies.

---

<p align="center">
  <sub>Windows Security Research - Browser Data Protection - Native C++ and Node.js</sub>
</p>
