---
authors:
  - name: Aaron Williamson
  - url: https://github.com/copiesofcopies
title: "Reference FOSS Policy"
tags:
  - Legal (Role)
sidebar_label: Policy (Reference)
---


<BoxOut title="Warning: Possibly out-of-date" image="/img/bok/roles/ospo.png">

This is content originally from the [FINOS Reference FOSS Policy Project](https://github.com/finos/reference-foss-policy) which has not been updated recently.  Feel free to suggest edits.

</BoxOut>

The Company supports certain activities associated with the contribution and publication of Free and Open Source Software (FOSS), when doing so is a benefit to the Company and does not present unacceptable risk. Risks include inadvertently disclosing sensitive information, giving up exclusive rights to intellectual property, infringement of third-party rights, and reputational harm.

These guidelines establish the minimum activities, approvals, restrictions, and evidence of compliance to be covered by the associated governance processes.

## Governance

<a id="ospo"></a>

### Open Source Program Office (OSPO)

The procedures and governance processes described in these guidelines are overseen by the Chair of the Open Source Program Office (OSPO).

The Open Source Program Office (OSPO) is responsible for establishing, evolving, and executing Free and Open Source Software (FOSS) contribution strategy and governance at the Company under the direction of the guidelines owner.

<a id="fosscontributionrisk"></a>

### FOSS Contribution Risk

Contributing to FOSS projects presents several risks. Preventative and detective internal controls must be implemented to address risks which apply to FOSS contribution activities. In addition, risks which are specific to participation in a particular FOSS project must be identified and recorded, and preventative and detective internal controls implemented as defined in these guidelines.

For guidance, the main risks are:

1.  **Data Leakage** - this includes unauthorized disclosure of non-public information and client data, unauthorized disclosure of internal security procedures, internal information such as network structures, IP addresses, server names, key material, authentication data, etc.  
    
2.  **Financial Loss** - contributing software to FOSS projects under most acceptable FOSS licenses involves granting a perpetual, royalty free licenses to consumers of the FOSS project and therefore account must be made of any financial write down of the software asset.

3.  **Intellectual Property (IP)** - Consideration must be made before contributing works to FOSS projects as to whether the Company should retain Intellectual Property rights over any parts of the works including whether Trademarks and/or Patents should be applied for **in advance**.

4.  **Reputational Damage** - There are several risks that could reflect poorly on the Company's brand and reputation, ranging from the decision to collaborate in a project, the quality of code contributed, remarks, opinions and other representations attributed to the Company, employees, and projects being abandoned through lack of investment.

5.  **Conflict of Interest Risk** - Risk that the Company employees are engaged in business activities or interests outside the scope of their permitted FOSS contribution activities that interfere with or compromise, or appear to interfere with or compromise, their ability to act in the best interest of the Company and/or its clients.

In addition, there are several consequential risks which must be considered that involve one more of the main risks:

1.  **FOSS License Compliance** - Non-compliance with FOSS licenses can expose the Company to several risks including litigation, reputational damage, and financial loss.  
    
2.  **FOSS License Permissions, Warranty and Liability** - There are a myriad of open source licenses, each with differing permissions, restrictions and conditions which can protect or expose the Company to litigation or restrict our ability to claim patent or trademark rights.  
    
3.  **Non-Compliance with relevant Company Polices** - These are discussed in [Specific Alignment with Relevant Regulations](#regulationalignment) and include regulatory commitments such as Export and Trade Controls, and Cross Border Data Flows.

<br /> 

<a id="standardrequirements"></a>

### Standard Requirements

The Company supports contribution and publication of Free and Open Source Software (FOSS) within the limits of these guidelines.

<a id="terminology"></a>

#### Terminology

FOSS terms can conflict with established definitions, for example: _Initiative_, _Program_, and _Project_ are well established Program and Project Management terms. For clarity, terms used in these guidelines shall refer to FOSS.

<a id="taxonomy"></a>

#### Taxonomy - Open Source Contribution

The Company has established a taxonomy to be used in conjunction with these guidelines and associated procedures.

<a id="fossprojectcategories"></a>

### FOSS Project Categories
 
Contributions made to FOSS projects by Company employees must fall into one of four categories below and meet the corresponding requirements for the category.

| **Category** | **Description** |
| --- | --- |
| Company Moderated | Open-source projects initiated by the Company where the Company will act as the primary project moderator/maintainer. These can be complete software solutions, open standards proposals, or simple functions. | 
| Company Interest (Major) | Open-source projects consumed in Company applications, moderated by a non-Company entity, where: <br /> 1.  The Company wishes to influence the direction of the FOSS project or, <br /> 2.  The Company wishes to contribute significant functionality that would benefit The Company and the project. <br /> <br /> These can be complete software solutions, open standards proposals, or simple functions. |
| Company Interest (Minor) | Open-source projects consumed in Company applications, moderated by a non-Company entity, where: <br /> 1.  The Company does not wish to influence the direction of the project but, <br /> 2.  The Company benefits by allowing employees to contribute. <br /> <br /> Examples include small enhancements and bug fixes to FOSS commonly used within Company applications to avoid the need for internal forks to work around defects. |
| Personal Contribution | An open-source work effort conducted by Company employees outside of their regular Company-contracted activities to FOSS projects that are not categorized as Company Moderated or Company Interest and for which there is no benefit to the company in contributing. |

*Table 1: Project Categories*

<a id="companyinfrastructure"></a>

## Company Infrastructure

1.  Company Moderated and Company Interest FOSS contribution activities may be performed within or outside of the Company's network.
2.  Personal FOSS contributions must be performed outside the Company's network using non-Company managed hardware.
3.  External infrastructure used to host Company Moderated projects must be approved by the OSPO.

<a id="ospostandardtools"></a> 

### OSPO Standard Tools

1.  Preventative and detective internal controls must be implemented to address the risks described in [FOSS Contribution Risk](#fosscontributionrisk).
2.  Company Moderated and Company Interest FOSS contribution activities must use OSPO approved Standard Tools when performing contributions within the Company's network or on Company managed hardware.
3.  These guidelines impose no tooling restrictions when making contributions outside the Company's network on non-Company managed hardware other than defined in [Company Infrastructure](#companyinfrastructure).
4.  These guidelines imposes no tooling restrictions for Personal contributions other than defined in [Company Infrastructure](#companyinfrastructure).
5.  Company Moderated FOSS projects are required to use an OSPO approved source code management tool.
6.  Company Moderated FOSS projects must maintain a transaction history showing evidence of the peer review, approver, and date must be maintained.
7.  The source code management, peer review, and scan requirements for Company Interest projects are defined by the relevant FOSS community.
8.  All contribution activities which occur from within the Company network or on the Company managed hardware must be subject to compliance scanning and review. This includes manual or automated processes to validate:
    1.  FOSS license compliance
    2.  Maker/checker tools (e.g., Peer reviewer not the same person as contributor)
    3.  Scans to reduce the risk of disclosing the Company non-public information, open source license violation, validated copyright text., and export regulations compliance.

:::warning
Company Moderated and Company Interest FOSS contribution activity must be registered in an OSPO approved inventory system
:::

#### Free and Open Source Software Consumption

These guidelines do not introduce or change established requirements for the introduction and consumption of free and open source software.

#### FOSS Identity

1.  Company employees are required to establish an identity on the publicly accessible platform used to host the FOSS project in accordance with the below:
2.  Contributors to Company Moderated and Company Interest projects must identify contributions using their Company external email address (e.g., john.doe@company.com) while employed at the Company. Contributors cannot use their Company internal email address or internal username.
3.  On cessation of employment by the Company, contributors must not tag commits with their Company email.
4.  Contributors to Personal Contribution projects must not use an identity that can be associated to the Company, for example Company external or internal email address or internal username.

#### Compliance with the Code of Conduct and related Policies

Employees must be made aware that their FOSS contribution activities must be in compliance with company conduct requirements which includes compliance with local laws and regulations at all times.

<a id="regulationalignment"></a> 

### Specific Alignment with Relevant Regulations

#### Identity and Access Management

Identity and Access Management requirements do not apply to externally hosted tooling platforms leveraged by FOSS contribution efforts. FOSS contribution and governance activities internal to the Company must comply with the Identity and Access Management requirements.

#### Records Management

The Company is obligated to retain certain records for legal, regulatory, or approved business reasons. This does not apply to FOSS contribution activities, and does apply to OSPO governance activities.

<a id="technologyexportimportregulations"></a> 

#### Technology Export/Import Regulations

Open source development is a global activity that makes software publicly available across national boundaries. Some countries may require FOSS project contributions to satisfy their local export control regulations. This is described in more detail in [Technology Export Regulations Compliance](#technologyexportregulationscompliance).

#### Information Classification

Open source contributions for Company Moderated and Company Interest project categories must be reviewed and approved for publication prior to transmitting out of the Company network:

1.  Contributions must be associated to an inventoried FOSS project registered in the OSPO FOSS inventory.
2.  Contributions containing material non-public information, non-standard cryptography (as defined in [Technology Export Regulations Compliance](#technologyexportregulationscompliance)), or non-standard authentication mechanisms must be remediated (e.g., have sensitive information removed) before approval.

#### Cross Border Data Flows

Many countries impose regulatory requirements governing the flow of personal data outside of their jurisdiction.

1.  These do not apply to FOSS contributions which include only the following activities:
    1.  Contributing source code or documentation which has been classified by the Company as public prior to contribution,
    2.  Participating in working group meetings with non-Company participants where the subject matter does not include Company internal business matters,
    3.  The use of data classified by the Company as public.
2.  These do apply to all other FOSS Contributions that do not qualify under those activities listed above including FOSS Contribution activities which contain data in the clear or data that is anonymized or de-identified. These activities must be approved prior to contribution.

#### Corporate Communications

Company Moderated or Company Interest project engagements which result in press releases or other public announcements must be approved.

#### Electronic Communications

The Company has a regulatory obligation to retain records of specific telephone conversations and electronic communications that relate to the reception, transmission and execution of client orders and proprietary trading, including communications that are intended to result in a business transaction, even if ultimately they do not.

Company Moderated, Company Interest and Personal Contribution project activities are general in nature. They must never discuss Company business and are therefore out of scope of these regulations.

Electronic communications conducted within the Company's network on Company managed hardware must use approved channels and must never discuss Company business.

Electronic communications conducted outside the Company's network on non-Company managed hardware are not subject to these restrictions but must never discuss Company business.

#### Third-party Management

A third-party relationship refers to the provision of services or products or other ongoing business relationship between the Company and a third-party, as described within one or more legal agreements that specifically outline the products, services, and performance expectations of the third-party.

1.  Company staff contributing to open-source communities is distinguishable from third-party performance and expectations therefore out of scope.
2.  Company Moderated projects that rely on externally hosted repositories and tools to support contributions are in scope.

<br /> 

<a id="governanceactivities"></a>

### Governance Activities

:::warning
FOSS projects must be reviewed and approved by the OSPO before contributions can be made. Company contributions are prohibited when the OSPO withdraws their approval, or the FOSS project is retired/archived. OSPO review does not apply to Personal Contributions (see [FOSS Project Categories](#fossprojectcategories)).
:::

#### FOSS License Inventory and Management

Free and Open-Source licenses are a legal agreement between the author(s) and consumers which dictate the terms and conditions that come with the use, modification, and distribution of the software.

1.  The OSPO must maintain an inventory of FOSS licenses approved for contribution activity by the Company contributors.
2.  The inventory must provide an auditable workflow of Legal review and Business approval or rejection of licenses for contribution activities detailing their Permissions, Conditions and Limitations.
3.  Review and approval or rejection of licenses for contribution activities must address the risks described in [FOSS Contribution Risk](#fosscontributionrisk).

#### Company-Moderated and Company Interest (Major) Projects

##### Opportunity Assessment and Registration

1.  All requests to participate and contribute to FOSS projects must be logged in an OSPO-approved tool.
2.  The OSPO must review and approve the conditions of the Foundation or community membership. This includes seeking Legal review and accepting any identified risks related to CLAs/CCLAs (if applicable).
3.  The request must include an intellectual property and competing interest review, and determine if there is a need for a trademark or patent application prior to commencing contribution.
4.  The request must include approval from a manager with budgetary control who can accept financial write-down of the works potentially being contributed.
5.  If the project license is not approved in the inventory, the OSPO must seek Legal review and categorization of the license.

##### OSPO Review and Decision

1.  The OSPO shall review requests and return a disposition based on advice from Legal and other SMEs where required.
2.  The OSPO has decision-making authority over requests and must record its decision in the system of record.

##### Initiation

FOSS projects may be supported by a stand-alone community or exist under a parent organization (for example, the Linux Foundation).

1.  Where the project is managed under a parent organization, the OSPO will appoint a Foundation Administrator to maintain the Company's relationship with the parent organization in good order and in compliance with the organization's charter.
2.  Once the Foundation relationship has been established, the Foundation Administrator must appoint a FOSS Project Administrator to maintain the Company's relationship with the project(s) in good order. This includes compliance with its charter and license requirements.
3.  For stand-alone FOSS projects that are not maintained under a parent organization, the OSPO will appoint a Non-Foundation Administrator who will oversee governance of all projects of this type. The Non-Foundation Administrator must appoint a FOSS Project Administrator to establish and maintain the Company's relationship with the project(s) in good order.

##### Maintenance

1.  FOSS Foundation Administrators, Non-Foundation Administrators, Project Administrators, and related staff must monitor their engagements for relevant risk changes (e.g., inactive projects, license changes, cross-border impacts, export regulation changes etc.).
2.  Potential changes in risk must be captured in the FOSS inventory upon identification, and the responsible Project Administrator must engage the relevant SMEs (e.g., Legal, Cross-Border etc.) for an impact assessment of the change.
3.  An OSPO review must be conducted when a potential change in risk has been captured in the FOSS inventory The disposition and actions taken must be recorded in the FOSS inventory.
4.  The OSPO must ensure all FOSS engagements are reviewed by the appointed FOSS Foundation Administrators, Non-Foundation Administrators or Project Administrators at least annually to identify material risk changes to the status of the FOSS engagement. The disposition and actions taken must be recorded in the FOSS Inventory.
5.  Foundation Administrators must prepare retirement/migration requests for FOSS projects we wish to transition. These must be reviewed by the OSPO, and the disposition and actions taken must be recorded in the FOSS Inventory.

##### Transition/Retire

1.  A decision to disengage from a FOSS project, FOSS Foundation or open source community must be reviewed and approved by the OSPO.
2.  An effective date must be agreed upon and recorded in the FOSS inventory having been petitioned by the stakeholder.
3.  On determining that the Company no longer has an interest in a Company Moderated project, the project must either be transitioned to a non-Company community for on-going maintenance or archived. The conduct of these activities must avoid brand and reputational risk to the Company.
4.  Administrators of retired FOSS Foundations and projects must ensure entitlements are removed from OSPO-approved tooling to ensure contribution cannot be conducted using the Company infrastructure on the agreed effective date.

##### Closed

The open source engagement or project must be successfully transitioned or retired on the agreed effective date and closure recorded in the FOSS inventory.

#### Company Interest (Minor) Projects

##### Opportunity Assessment and Registration

1.  Requests by any Company employee for access to contribute to a Company Interest (Minor) FOSS project must be submitted and recorded using an OSPO-approved tool.
2.  Contributions to Company Interest (Minor) do not require explicit OSPO approval if the FOSS product is approved for use by Company applications in the Company's official third-party product inventory, and the Open Source license associated with the FOSS project is present in the OSPO license inventory system and is approved for contribution.
3.  Company Interest (Minor) Projects may not be used to publish the Company patentable or trademarked contributions.
4.  The FOSS project access request must be classified as Company Interest (Minor) and address the requirements appropriate to the FOSS Project category.
5.  The requestor's line manager must approve the access request using the OSPO-approved tool, and must ensure the following requirements are met:
    1.  The FOSS product is approved for use by the Company applications in the Company's official product inventory.
    2.  It is beneficial to the Company to allow the requestor to contribute to the project (for example, the project is used in a business application developed by the requestor).
    3.  If the project requires contributors to agree to a Contributor License Agreement, Developer Certificate of Origin, or similar agreement, Legal must be engaged via the OSPO for advice.
    4.  Performing an intellectual property and competing interest review to determine the need for a trademark or patent application prior to commencing contribution.

##### OSPO Review and Decision

1.  Contribution access requests to FOSS projects must be associated to an approved license in the OSPO license inventory.
2.  The OSPO has decision-making authority over access requests and must record its decision in the system of record if appropriate.

##### Maintenance

1.  Project access requests must be recertified at least annually.
2.  The project's open source license must be validated regularly to identify, record, and re-assess the impact license changes.

<a id="transitionretire"></a> 

##### Transition/Retire

FOSS contribution projects and any associated access requests configured in the OSPO-approved tooling must be decommissioned within 3 months of that project being retired or archived from its public repository or the Company's official product inventory.

#### Personal Contribution Projects

Company employees may contribute to FOSS projects in a personal capacity under the following conditions:

1.  The FOSS project is not registered as a Company Moderated or Company Interest project in the FOSS Inventory.
2.  Contribution to the project and engagement with the project community does not conflict with the code of conduct.
3.  Contribution to the project and engagement with the project community must not represent a conflict of interest with Company business.
4.  Contribution to the project and engagement with the project community must not leverage Company intellectual property.
5.  Contribution to the project and engagement with the project community must adhere to use of social media guidelines.
6.  Contributors may not represent themselves as Company employees.
7.  Contributions must not be made from Company-owned hardware or infrastructure.

<a id="technologyexportregulationscompliance"></a> 

#### Technology Export Regulations Compliance

1.  Company-Moderated, Company Interest projects which provide or perform non-standard [\[1\]](#footnote-1) cryptography must be reviewed prior to OSPO approval (see [Technology Export/Import Regulations](#technologyexportimportregulations)).
2.  Company staff participating in FOSS contribution activities must comply with local export regulations.

<a id="contributionactivities"></a>

### Contribution Activities

1.  For all contribution activities which occur from within the Company network or on Company managed hardware, OSPO approved controls must be implemented to mitigate the risks described in [FOSS Contribution Risk](#fosscontributionrisk).
2.  FOSS contributions made from Company managed hardware or executed on the Company's network must use Company approved tools.
3.  FOSS Contributions made from non-Company hardware outside of the Company's network are not restricted to the use of tools.

#### Company Moderated Projects

1.  A FOSS Project team must be established consisting of the roles defined in [Roles & Responsibilities](#rolesandresponsiilities).
2.  The FOSS Project Team must define and document OSPO approved instructions describing how to report security vulnerabilities in the project [\[2\]](#footnote-2).
3.  Projects which are no longer moderated by a Company employee must be transitioned to Company Interest or Retired following the process described in Section [Transition/Retire](#transitionretire).

#### Company Interest (Major) Projects

1.  A FOSS Project team must be established consisting of the applicable roles defined in [Roles & Responsibilities](#rolesandresponsiilities).
2.  Activities must follow the contribution processes established by the project community.

#### Company Interest (Minor) Projects

Activities must follow contribution processes established by the project community.

<a id="training"></a>

## Training

Company staff participating in FOSS contribution activities as defined in these guidelines are required to complete an annual training class to demonstrate knowledge of these guidelines and associated governance consistent with their role.

<a id="rolesandresponsiilities"></a> 

## Roles & Responsibilities

Roles and responsibilities for these guidelines include:

| **Role** | **Project Category** | **Responsibility** |
| --- | --- | --- |
| Open Source Program Office (OSPO) <br /> <br /> (Chair/Members) | Company Moderated <br /> <br /> Company Interest (Major) <br /> <br /> Company Interest (Minor) | Committee responsible for maintaining the Open Source Contribution guidelines. |
| Line Manager | Company Interest (Minor) | Approver of Company Interest Minor FOSS contribution requests via OSPO tooling. |
| FOSS Project Moderator or Maintainer | Company Moderated <br /> <br /> Company Interest (Major) | <p>Establishing and ensuring the community adheres to:</p><ul><li>The OSPO approved community code of conduct, and</li><li>Formal contribution processes which can include defining other community activities and pull request approvals.</li></ul> |
| FOSS Sponsor | Company Moderated <br /> <br /> Company Interest (Major) | Responsible for sponsoring the project including a documented business case, financial commitment and budget approval, intellectual property and competing interest review, and determining a need for trademark or patent applications. |
| FOSS Contributor| Company Moderated <br /> <br /> Company Interest (Major) <br /> <br /> Company Interest (Minor) | A FOSS community term which refers to any person who contributes to a FOSS project in any capacity. Under the terms of these guidelines, it is specific to Company employees contributing to FOSS projects. |
| FOSS Project Administrator | Company Moderated <br /> <br /> Company Interest (Major) | Ensuring the control requirements of these guidelines are met and evidenced for their FOSS project(s) |
| FOSS Foundation Administrator | Company Moderated <br /> <br /> Company Interest (Major) | Ensuring the control requirements of these guidelines are met and evidenced for the Company's membership of FOSS Foundations. |

*Table 2: Roles*

<a id="legalsupport"></a>

## Legal Support

Free and Open-Source licenses are legal agreements between the author(s) and consumers. The OSPO maintains an inventory of FOSS licenses approved for contribution activity by Company contributors. The legal department's role is advisory to the OSPO. The OSPO engages legal as needed when adding a new license to the inventory, when changes occur to an existing license, when project contributors must first agree to a Contributor License Agreement, Developer Certificate of Origin, or similar agreement. Legal review activities and disposition will be captured and timestamped by the OSPO.

<br /> 

<a id="appendix"></a>

## Appendix A - Glossary 

| **Term** | **Definition** |
| --- | --- |
| Contributor License Agreement (CLA) | A contract between the FOSS project and either an individual developer or the company contributing code. CLAs may be categorized as Individual CLAs or Corporate CLAs (CCLA). |
| Individual CLA | An individual developer agrees they have the right to contribute code and binds their contributions to the FOSS project under the terms of the CLA. |
| Corporate CLA | Provide direct corporate authority for employees of a company to make contributions with explicit authority for a patent grant in an open source license. Corporate CLAs must be signed by an authorized signatory to be valid. |
| Developer Certificate of Origin (DCO) | A per commit sign-off made by a contributor indicating they agree to the terms published at <a href="https://developercertificate.org">https://developercertificate.org</a> for that particular contribution. |
| FOSS Community | Free and Open Source Software (FOSS); Free from most constraints on copyrights and cost. Software is made available under an Open Source Definition (OSD) compliant license in source code form to facilitate modification. "FOSS" and "Open Source" are interchangeable. <br /> <br /> A FOSS Community is group of authorized individuals with contribution/review entitlement to a FOSS project. The FOSS project can be organized as part of a foundation or for-profit entity (e.g., corporation).|
| (The) Open Source Definition (OSD) | A document published by the <a href="https://opensource.org/about">Open Source Initiative</a> (OSI) used to determine if a license can be labeled with the Open Source Certification mark. |
| Open Source Foundation (Organizations) | Not for profit and charitable organizations providing a neutral playing field for developers, technologists, and companies to collectively contribute to common solutions and growth. Notable foundations include The Apache Software Foundation, Cloud Native Computing Foundation, Eclipse Foundation, Free Software Foundation, Mozilla Foundation, and the Open Source Initiative. |

*Table 3: Glossary*
