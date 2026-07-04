# Security Policy

## Scope

This repository publishes a static, client-side single HTML application.

The project does not include a server-side API, authentication system, database,
secret management system, payment flow, or user account system.

## Reporting policy

This repository is maintained primarily as a read-only public demo and reference
implementation.

The repository owner does not publish a personal email address or other personal
contact information for security reports.

Issues and Pull requests are intended to be disabled through GitHub repository
settings. Please do not use public repository features for security-sensitive
reports.

No dedicated vulnerability reporting channel is provided for this repository.
If the repository owner later enables an official private reporting channel,
this policy should be updated accordingly.

## Current security model

The reviewed public build is designed to run entirely in the browser.

Static review of the application-specific code found no intentional use of:

- external runtime CDN loading
- runtime Babel transformation
- `fetch`
- `XMLHttpRequest`
- `WebSocket`
- `navigator.sendBeacon`
- `localStorage`
- `sessionStorage`
- `indexedDB`
- `document.cookie`
- HTML forms

The application intentionally uses browser-side APIs such as WebGL, Web Worker,
Blob URLs, `URL.createObjectURL`, `postMessage`, and optional vibration feedback
for local simulation and rendering.

Bundled third-party libraries may contain generic loader or DOM utility code that
is not used as an application-level external communication feature.

## Maintenance note

The main publication focus of this repository is license compliance and proper
attribution for redistributed third-party JavaScript/CSS libraries.

If future versions add networking, user data handling, authentication, external
APIs, analytics, or server-side components, this policy should be reviewed and
updated before release.
