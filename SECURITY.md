# Security Policy

The **Shoaib Aftab CSS Framework** is designed with a "Secure by Default" architecture. It is built to meet the rigorous demands of enterprise applications, banking systems, and high-security government portals.

## Supported Versions

Currently, the following versions are supported with security patches:

| Version | Supported          |
| ------- | ------------------ |
| 2.0.x   | :white_check_mark: |
| 1.0.x   | :x:                |

## Security Features

1. **Air-Gapped & Zero Dependency Compatibility**
   The framework relies on 0 external packages. There are no NPM dependency trees that could be compromised via supply-chain attacks. It is 100% self-contained.

2. **ReDoS Protected Build System**
   The custom native CSS minifier `scripts/build.js` uses strictly linear Regular Expressions (e.g. `\/\*[\s\S]*?\*\/`) to prevent Catastrophic Backtracking / Regular Expression Denial of Service (ReDoS) attacks during CI/CD pipelines.

3. **No Dynamic Execution**
   The framework contains absolutely no dynamic script execution mechanisms (such as old IE `expression()` or `behavior: url(...)` properties).

4. **Zero Cross-Origin Leaks**
   We enforce a strict policy against external `@import` rules and remote `url()` assets to prevent MITM attacks and third-party tracking.

## Reporting a Vulnerability

If you discover a vulnerability, please do NOT open a public issue. We take security seriously and ask that you report it privately.

**Email:** security@shoaib-aftab-tech.com

We will acknowledge your email within 24 hours and issue a patch (if required) within 72 hours.
