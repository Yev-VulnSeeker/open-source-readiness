---
title: Open Source Supply Chain Security Testing
tags: 
  - Developer (Role)
  - Risk-Compliance (Role)
  - Security Expert (Role)
  - CIO (Role)
  - Placeholder
  - Codebase Risk
  - Dependency Risk
  - Operational Risk
  - Level 2 (OSMM) 
sidebar_position: 4
sidebar_label: Security
---
**THIS IS A PLACEHOLDER**

- EU Cyber Resilience Act
- https://www.congress.gov/bill/117th-congress/senate-bill/4913
- https://openssf.org/blog/2022/09/27/the-united-states-securing-open-source-software-act-what-you-need-to-know/ (govt sector)
- find the UK act that also does this.


Regarding threat models: I think this is something we could review as a group.

There are some here: https://cloud.google.com/software-supply-chain-security/docs/attack-vectors
Some on page 6 of this: https://github.com/ossf/s2c2f/blob/main/specification/Secure_Supply_Chain_Consumption_Framework_(S2C2F).pdf
And some in The Mitre Att&ck Model
Probably more in FS-ISAC (although as a non-member I can't read it)
Also, a talk I attended by Eclipse Foundation detailed a few others that seem novel.
Is there a definitively maintained list anywhere?

Also useful:

SLSA
Supply Chain Best Practices

OpenSSF

tbd: break into _incoming_ and _outgoing_

include:
 - Vulnerability Testing
 - keeping dependencies up-to-date https://openssf.org/resources/guides/
 

- KPIs around dependencies?

- code reviews (GGI)


Security testing is a broad term that encompasses various techniques for evaluating the security of software systems and applications. The main types of security testing include:

1. Software Composition Analysis (SCA) or Vulnerability Scanning: Vulnerability scanning involves automatically searching for known security weaknesses in software systems and applications. This type of testing can help identify potential security risks, but does not guarantee that all vulnerabilities have been found.
2. Static Application Security Testing (SAST): SAST involves analyzing the source code of an application for potential security vulnerabilities without executing the code. This type of testing can help identify potential security risks early in the development process, before the code is deployed.
3. Dynamic Application Security Testing (DAST): DAST involves executing the code of an application and examining its behavior for potential security vulnerabilities. This type of testing can help identify potential security risks that may not be apparent from examining the code alone.
4. Penetration Testing: Penetration testing involves attempting to actively exploit vulnerabilities in a software system or application to determine its security weaknesses. This type of testing is usually conducted by security experts who use manual and automated techniques to simulate real-world attacks.
5. Web Application Security Testing: Web application security testing focuses on identifying security vulnerabilities in web applications, such as SQL injection, cross-site scripting (XSS), and cross-site request forgery (CSRF).
6. Infrastructure Security Testing: Infrastructure security testing involves evaluating the security of the underlying infrastructure that supports a software system or application, such as networks, servers, and databases.
7. Mobile Application Security Testing: Mobile application security testing focuses on identifying security vulnerabilities in mobile applications, such as those running on iOS or Android platforms.

## Software Composition Analysis

According to https://en.wikipedia.org/wiki/Software_Composition_Analysis:

> **Software Composition Analysis** (SCA) is a practice in the fields of [Information technology](https://en.wikipedia.org/wiki/Information_technology) and [software engineering](https://en.wikipedia.org/wiki/Software_engineering) for analyzing custom-built software applications to detect embedded open-source software and detect if they are up-to-date, contain security flaws, or have licensing requirements.

Many SCA tools produce SBOMs which can then be checked for vulnerabilities.   A long list is provided here: https://todogroup.org/guides/management-tools/#tools-for-managing-source-code

## Static Application Security Testing

See: https://snyk.io/learn/application-security/static-application-security-testing/

SAST, or Static Application Security Testing, is a type of software security testing that analyzes the source code of an application for potential security vulnerabilities without executing the code. The leading SAST tools are:

1. Checkmarx: Checkmarx is a commercial SAST tool that provides a comprehensive solution for finding security vulnerabilities in source code. It supports a wide range of programming languages and provides detailed analysis of potential security issues.
2. Veracode: Veracode is a commercial SAST tool that provides a cloud-based solution for finding security vulnerabilities in source code. It integrates with a variety of development tools and provides a range of reporting and remediation options.
3. SonarQube: SonarQube is an open source platform for continuous inspection of code quality and security. It provides a range of tools for code analysis, including SAST capabilities, and supports a wide range of programming languages.
4. Fortify: Fortify is a commercial SAST tool that provides a comprehensive solution for finding security vulnerabilities in source code. It supports a wide range of programming languages and provides detailed analysis of potential security issues.
5. Coverity: Coverity is a commercial SAST tool that provides a comprehensive solution for finding security vulnerabilities in source code. It supports a wide range of programming languages and provides detailed analysis of potential security issues.

tbd.

## Dynamic Application Security Testing 


tbd.

## Initiatives

- **[SLSA](https://slsa.dev/spec/v1.0/threats-overview)**: "Supply chain Levels for Software Artifacts".  This is a framework designed for creating repeatable builds with provenance of their components.

- **[OpenChain]( https://www.openchainproject.org/)**:  an ISO standard for open source license compliance, developed and hosted by the Linux Foundation. It provides a set of requirements to create effective open source management systems, helping companies to minimize legal risks related to open source software use and improve efficiency and trust in the software supply chain.

- **[Renovate Bot](https://docs.renovatebot.com)**: Renovate Bot is an open-source tool that helps to automate the process of updating dependencies in software projects. It scans your project for dependencies, automatically opens pull requests to update outdated ones, and provides change logs and compatibility information to assist in validation and troubleshooting.

- **[Secure Supply Chain Consumption Framework (S23C2F)](https://github.com/ossf/s2c2f)**: The S2C2F SIG is a group working within the OpenSSF's Supply Chain Integrity Working Group formed to further develop and continuously improve the [S2C2F guide](https://github.com/ossf/s2c2f/blob/main/specification/Secure_Supply_Chain_Consumption_Framework_(S2C2F).pdf) which outlines and defines how to securely consume Open Source Software (OSS) dependencies into the developer’s workflow.

- **[Financial Services Information Sharing and Analysis Center (FS-ISAC)](https://www.fsisac.com)**:  a non-profit organization dedicated to reducing cyber-risk in the global financial system. It enables members to share threat and vulnerability information, collaborate on incident response and mitigation, conduct synchronized response, and provides tools for better protection against physical and cyber threats.

## OSPO Alliance Talk

Mikael Barbero (Eclipse)
Florent Zara
Stefano Pampaloni - said hi

Attendees (About 15) - Orange, OmniCloud, Amadeus

Attending State Of Open Con!

Talk on Open Source Security:

- Exponential increase in attacks
- Solar WInds - 95% of the Fortune 500.
- Approaches:
    - Dodgy Commits introducing use-after-free
    - Impersonation
    - Maintainer change to someone less scrupulous
    - Dodgy build servers/git hosts
    - Repo-jacking (github actions, changing usernames on GitHub
    - Dependencies (log4shell)
    - typosquatting (e.g. electorn)
    - dependency confusion - internal/external dependencies with wrong versions
    - leaked credentials (codecov)
    - Star Jacking (django-filer) - link the wrong github repo and have their stars/readme (npm issue)
    - "Joke" Deps - not considered a supply-chain security issue
- Provenance Attestation - checking the signature of the dep
- Code signing, 2fa
- Removing inactive accounts
- Legislation (coming, EU and US) - enforcing developer responsibility. somewhat threatening the OSS community.

### SLSA: Supply Chain for Software Artifacts

Signed provenance, security controls on host.  this looks pretty cool
Generated SBOMs

### Open SSF

[github.com/ossf/scorecard](http://github.com/ossf/scorecard)
[github.com/ossf/allstar](http://github.com/ossf/allstar)

Our tools!

### FINOS Supply Chain Security 20 Jun 2023

- https://www.fsisac.com
- https://github.com/ossf/s2c2f

## From Mark

 - https://www.gartner.com/reviews/market/security-threat-intelligence-services
 - https://www.crunchbase.com/organization/digital-shadows
