# Security

## Reporting a vulnerability

Please do not report security vulnerabilities through public GitHub issues.

Report security vulnerabilities to:

**support@herego.video**

Please include:

- a description of the vulnerability;
- the affected endpoint or component;
- steps to reproduce where possible;
- potential impact.

## Request access tokens

HereGo request access tokens authorize access to a specific video request and its associated submitted video.

Treat these tokens as secrets.

Do not:

- commit tokens to source control;
- include tokens in public issues or pull requests;
- log tokens unnecessarily;
- expose tokens in analytics or telemetry.

The request access token is intentionally returned to the calling agent because it is required for subsequent access to the request and video.

## Video privacy

HereGo videos are served through authenticated API endpoints.

Underlying storage URLs are not exposed as permanent public media URLs.

Video access ends when the associated request/video expires.

Clients should not assume that expiry can revoke copies of video bytes that were already downloaded.
