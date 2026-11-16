# Penetration Testing Report: arngren.net

## Overview
This repository contains a comprehensive security assessment and penetration testing report for the website **arngren.net**. 
The assessment was conducted using the **PTES** (Penetration Testing Execution Standard) methodology to evaluate the website's security posture and identify potential vulnerabilities.

## Authors
- Mohammed Abdo Haron Habbat

## Key Findings Summary
The assessment revealed several security observations ranging from Low to Medium severity. The detailed findings are documented in the uploaded PDF report, including:

1. **DNSSEC is not enabled (Medium):** The domain is unsigned, increasing the risk of DNS spoofing and cache poisoning attacks.
2. **Missing Registrar Lock (Medium):** The domain lacks `clientTransferProhibited` status, making it vulnerable to unauthorized domain transfers (Domain Hijacking).

## Methodology & Tools Used
- **PTES Methodology:** Followed for structured penetration testing.
- **Ping:** To verify target availability and detect the operating system (TTL=128 indicates Windows).
- **WHOIS:** To gather domain registration information and identify DNS servers.
- **WhatWeb:** For web server fingerprinting (Identified Apache server, version hidden).
- **cURL:** To inspect HTTP headers and server responses (403 Forbidden detected).

## Repository Contents
- `Penetration_Test_Report.pdf`: The full detailed report in Arabic, including screenshots and technical analysis.
- `README.md`: Project overview and summary.
