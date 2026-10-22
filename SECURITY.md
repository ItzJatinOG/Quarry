# Security Policy

This repository is a public website and documentation project. It does not currently include a dedicated security reporting email or private vulnerability intake process. If the project owner later adds one, that channel should be documented here.

## Reporting a vulnerability

If you believe you have found a security issue in the repository, the website, or a related public service:

- do not publish the issue publicly before the owner has had a chance to assess it
- do not include credentials, secrets, tokens, private user content, or private endpoints in issue reports
- report the issue privately to the repository owner through a channel they have explicitly provided

If no private reporting channel is available yet, please keep the issue limited to public documentation or repository issues until the owner sets up a secure disclosure process.

## Safe development practices

- review generated code before running it in a real server environment
- do not execute untrusted plugin code on production worlds without testing it first
- keep backups before installing new plugins or changing server configuration
- treat generated plugin code as untrusted until it has been reviewed manually

## Website and repo hygiene

- do not commit credentials, secret keys, private environment variables, or API tokens
- do not include sensitive user data in examples or issue reports
- avoid exposing internal debugging data in public documentation

## Dependency and configuration security

- keep dependencies current where the project is managed by package or build tooling
- review generated or third-party code before integrating it into a production environment
- avoid running code from untrusted sources on a live server or public production system

## Current status

The repository currently does not contain a verified security reporting email address or private vulnerability intake mechanism. Until one exists, the safest approach is to report issues through the repository owner’s preferred private channel or to avoid disclosing sensitive details in public.
