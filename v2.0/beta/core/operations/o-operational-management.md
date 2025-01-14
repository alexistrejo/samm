---
business_functions : Operations
title : Operational Management
assignedto       : John (john.dileo@owasp.org)
complete          : 10%
business_functions_weight: 3
type: security_practice
---

# Overview
The Operational Management practice focuses on activities to ensure security is maintained throughout operational support functions. Although these functions are not performed directly by an application, the overall security of the application and its data is dependent on their proper performance. All of the protections built into an application can be rendered irrelevant by deploying the application on an unpatched system or failing to store backup media securely.

The functions covered by this practice include, but are not limited to: system provisioning, administration, and decommissioning; database provisioning and administration; and data backup, restore, and archival.

| | A: Data Protection | B: System decomissioning / Legacy management |
|:---|:---|:---|
| Maturity 1 - Foundational Practices | Data locations documented | Opportunistic identification of unused applications or services |
| Maturity 2 - Managed, Responsive Processes | Data protection policy established | Decomissioning process in place |
| Maturity 3 - Active Monitoring and Response | Data policy breaches detected and acted upon | Proactive reliable handling of legacy |

## Practice Notes
Possibly move the Third-Party Requirements stream into this practice, as a third stream?


# A: Data Protection

## Maturity 1
### Activity
The data stored, processed, and transmitted by the application are identified, and information regarding their types, sensitivity levels, and storage location(s) are captured. Data elements subject to specific regulation are clearly identified. Appropriate controls are in place to ensure sensitive data from Production environments are not propagated to lower environments without having been properly sanitized/anonymized.

The actions comprising this activity represent the minimum necessary level of awareness and safeguards, to be confident the organization understands the scope of existing data protection needs. By ensuring unsanitized production data are never propagated to lower (non-production) environments, the organization is able to focus data protection policies and activities on production. Full understanding of the data the organization works with is a prerequisite to developing actionable policies for their protection.

### Maturity Questions
#### Q 1
Are data catalogued, including their types, sensitivity levels, and processing/storage locations?

*Answer Options*

- No
- Yes, for a small percentage
- Yes, for approx. half
- Yes, for most or all

#### Q 2
Are controls in place to ensure sensitive data are sanitized before propagation to a non-production environment, and is compliance with those controls verified?

*Answer Options*

- No
- Yes, some of the time
- Yes, approx. half the time
- Yes, most or all of the time

## Maturity 2
### Activity
At this maturity level, Data Protection activities are focused on actively managing the organization's stewardship of data. Technical and administrative controls established as part of this Activity serve to protect the confidentiality of sensitive data, as well as the integrity and availability of all data in the organization's care, from its initial creation/receipt through the destruction of backups at the end of their retention period.

The organization has an established Data Protection Policy. Processes, procedures, and safeguards are in place for protecting and preserving data throughout their lifetime, whether at rest, being processed, or in transit. Particular attention is given to the handling and protection of sensitive data outside the active processing system, including, but not limited to: storage, retention, and destruction of backups; and the labeling, encryption, and physical protection of offline storage media. Organization processes and procedures are adapted to ensure compliance with regulatory, contractual, or other restrictions on storage locations, personnel access, and other factors.

### Maturity Questions
#### Q 1
Are retention requirements established for data, and are backups destroyed in a timely manner after the relevant retention period ends?

*Answer Options*

- No
- Yes, some of the time
- Yes, approx. half of the time
- Yes, most or all of the time

#### Q 2
Are handling requirements established and documented for all data elements in the catalog, in accordance with their established sensitivity levels, and are these requirements followed?

*Answer Options*

- No
- Yes, some of the time
- Yes, approx. half of the time
- Yes, most or all of the time

## Maturity 3
### Activity
Technical controls are implemented to enforce compliance with the Data Protection Policy, and active monitoring is in place to detect attempted or actual violations. The organization's compliance with established administrative controls is regularly checked/audited. Performance and operation of automated mechanisms, including backups and record deletions, is closely monitored; failures are quickly detected and reported, to ensure timely corrective action can be taken.

Activities at this maturity level are focused on making data protection "automatic," reducing the organization's reliance on human effort to assess and manage compliance with policies.

### Maturity Questions
#### Q 1
Is automated monitoring in place, to detect attempted or actual violations of the Data Protection Policy?

*Answer Options*

- No
- Yes, for some data
- Yes, for approx. half of the data
- Yes, for most or all of the data

#### Q 2
Are administrative data protection controls audited?

*Answer Options*

- No
- Yes, we did it once
- Yes, we do it every few years
- Yes, we do it at least annually


# B: System decomissioning / Legacy management

## Maturity 1
### Activity
Explicit (manual or automated) actions for identification of unused applications are carried out. Results are processed for further actions.

### Activity - Alpha Version
Explicit (manual or automated) actions for identification of unused applications are carried out. Results are processed for further actions.

### Maturity Questions
#### Q 1
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat?

*Answer Options*

- Option 1
- Option 2
- Option 3
- Option 4

#### Notes
definition of legacy ?
out of date or in need of replacement?
no active development / maintenance?

## Maturity 2
### Activity
If application is decomissioned, also all relevant accounts, firewall rules, data, etc. are deleted according to an established process.

### Activity - Alpha Version
If application is decomissioned, also all relevant accounts, firewall rules, data, etc. are deleted according to an established process.

### Maturity Questions
#### Q 1
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat?

*Answer Options*

- Option 1
- Option 2
- Option 3
- Option 4

#### Notes


## Maturity 3
### Activity
Life state of every software asset and underlying infrastructure is periodically evaluated and EOL is estimated. Switching the application into a legacy state triggers a defined process which also mitigates resulting security risks. Lessons learned process for handling legacy is established. 

### Activity - Alpha Version
Life state of every software asset and underlying infrastructure is periodically evaluated and EOL is estimated. Switching the application into a legacy state triggers a defined process which also mitigates resulting security risks. Lessons learned process for handling legacy is established. 

### Maturity Questions
#### Q 1
Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat?

*Answer Options*

- Option 1
- Option 2
- Option 3
- Option 4

#### Notes
Proactivity in driving infrastructure and application standards, to preemptively wean the enterprise from EOL technologies.
