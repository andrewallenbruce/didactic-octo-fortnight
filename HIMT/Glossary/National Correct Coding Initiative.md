---
tags: definition, him, cpt, coding, ncci, ncd, lcd, mue, glossary/him
alias: NCCI, CCI, national correct coding initiative, Correct Coding Initiative, correct coding initiative
---
# National Correct Coding Initiative (NCCI)
*Used by professional billers to determine codes considered by [[CMS]] to be bundled codes for procedures and services deemed necessary to accomplish a [[Major Surgery|major]] procedure. This is to promote correct coding methodologies and to control improper assignment of codes that results in inappropriate reimbursement.*

The National Correct Coding Initiative (NCCI) is a [[CMS]] program designed to prevent improper payment of procedures that should not be submitted together. NCCI, also shortened to CCI, is an automated [[edit]] system used to indicate specific [[Current Procedural Terminology|CPT]]® code pairs and whether they can be reported on the same date of service for the same [[beneficiary]] by the same provider. [[CMS]] implemented the NCCI to promote correct coding methodologies and to control improper assignment of codes resulting in inappropriate reimbursement. NCCI coding policies are based on:

- Analysis of standard medical and surgical practice
- Coding conventions included in CPT®
- Coding guidelines developed by national medical specialty societies through the CPT® Advisory Committee (committee members include representatives of major medical societies)
- Local and [[National Coverage Determination|national coverage determinations]]
- A review of current coding practices

The edits are updated quarterly by [[CMS]], and the policy manual is updated annually.
NCCI is used by professional coders and billers to determine codes considered by CMS to be bundled for procedures and services deemed necessary to accomplish a [[Major Surgery|major]] procedure. Bundled procedure codes are not reported separately. The components of a bundled procedure are included in the comprehensive procedure code.

```ad-billing
title: Billing
Beware: reporting bundled procedure codes in addition to the major procedure code is characterized as [[unbundling]] and, if repeated with enough frequency, could be considered an act of [[fraud]].
```

Local CMS carriers, ([[Medicare Administrative Contractor (MAC)]]s) began using the NCCI edits on January 1, 1996. Since October 2010, the [[Patient Protection and Affordable Care Act]] § 6507
([[Patient Protection and Affordable Care Act|ACA]]) required state Medicaid programs to incorporate NCCI methodologies into their claims processing. Many commercial health plans also utilize the NCCI edits in their claims processing. NCCI edits were originally developed to assist MACs in processing Medicare Part B claims. In August of 2000, NCCI edits were added to the [[Outpatient Code Editor]] (OCE) to assist MACs in processing Part B claims for outpatient hospital services.

## NCCI Edits
The NCCI includes two types of edits:
1. **Procedure to Procedure (PTP) edits**: PTP edits apply to code pairs that should not be billed together because one service inherently includes the other. In certain situations, an appropriate modifier may be allowed and used.  
	1. **Mutually exclusive edits (MEE)** are included in the PTP edits. These edits include code pairs that, for clinical reasons, are unlikely to be performed on the same patient on the same date of service. For example, two different types of laboratory testing that would produce the same result as one test.
2. **[[Medically Unlikely Edits]] (MUEs)**:  MUEs indicate a maximum number of Units of Service (UOS) allowable under most circumstances for a single CPT® or HCPCS Level II code billed by a provider on a single date of service for a [[beneficiary]].

The NCCI is composed of two Provider-type choices of code pair edits and three Provider-type choices of [[Medically Unlikely Edits|MUEs]].

### PTP Code Pair Edits
- NCCI Edits—Practitioners: code pair edits applied to claims submitted by physician, non-physician practitioners, and [[Ambulatory Surgery Center]]s (ASCs).
- NCCI Edits—Hospital: code pair edits applied to Types of Bills (TOBs) subject to the [[Outpatient Code Editor|OCE]]—Hospitals, Skilled Nursing Facilities, Home Health Agencies, Outpatient Physical Therapy and Speech-Language Pathology Providers, and Comprehensive Outpatient Rehabilitation Facilities.
- Medically Unlikely Edits ([[Medically Unlikely Edits|MUEs]]):
	- Practitioner [[Medically Unlikely Edits|MUEs]]: All physician and other practitioner claims are subject to these edits.
	- Durable Medical Equipment (DME) Supplier MUEs: These edits are applied to claims submitted to DME [[Medicare Administrative Contractor (MAC)|MACs]]. (At this time, this file will include HCPCS A-B and E-V codes, in addition to HCPCS codes under the DME [[Medicare Administrative Contractor (MAC)|MAC]] jurisdiction.)
	- Facility Outpatient MUEs: Claims for TOB 13X, 14X, and Critical Access Hospitals (85X) are subject to these edits.

Many NCCI edits are based on the standards of medical/surgical care. Services integral to another service are considered component parts of the more comprehensive service. The comprehensive codes are placed in column 1 and the component codes in column 2. Some services integral to many procedures include:
- Cleaning, shaving, and prepping of skin
- Draping and positioning the patient
- Insertion of urinary catheter
- Surgical approach
- Surgical cultures
- Surgical closure

According to the NCCI Policy Manual, there are general principles that can be applied to the edits:
1. The component (column 2) service is an accepted standard of care when performing the comprehensive (column 1) service.
2. The component service is usually necessary to complete the comprehensive service.
3. The component service is not a separately distinguishable procedure when performed with the comprehensive service.

Specific examples of services that are not separately reportable because they are components of more comprehensive services include:
- Medical: Since a cardiac stress test (codes 93015-93018) includes multiple electrocardiograms, an electrocardiogram (code 93005 or 93010) is not separately reportable.
- Surgical: Since a myringotomy (code 69421) requires access to the tympanic membrane (ear drum) through the external auditory canal (EAC), removal of impacted cerumen (code 69210) from the EAC is not separately reportable.
The component elements of the preoperative and postoperative work for each procedure are included component services of that procedure as a standard of medical/surgical practice. These include:
- insertion of a central venous access device
- cardiopulmonary monitoring
- exposure and exploration of the surgical field

#### PTP Table Example
![](https://i.imgur.com/JdKyCPp.png)
The Correct Coding file formats continue to include a Correct Coding Modifier (CCM) indicator (carrier only) for both the Comprehensive/Component Table. This indicator determines whether a CCM causes the code pair to bypass the edit. This indicator will be either “0,” “1,” or “9.” The definitions of each are:

| CCM Indicator | Definition                                                                                                                              |
| ------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| 0             | CCM not allowed and will not bypass edits                                                                                      |
| 1             | CCM is allowed and will bypass edits                                                                                              |
| 9             | NCCI edit does not apply to this PTP code pair |


##### Example 1
>11043, Debridement, muscle and/or fascia (includes epidermis, dermis, and subcutaneous tissue, if performed); first 20 sq. cm or less

can never be billed with codes 

>62320, Injection(s), of diagnostic or therapeutic substance(s)…cervical or thoracic, 

or 

>62321, Injection(s), of diagnostic or therapeutic substance(s)…cervical or thoracic; with imaging guidance.

Because the CCM indicator is 0, no [[modifier]] can be used to bypass the edits. In other words, you cannot bill these two codes together.

##### Example 2
>11042, Debridement, subcutaneous tissue (includes epidermis and dermis, if performed); first 20 square cm or less

may be billed with 

>11720, Debridement of nail(s) by any method(s); 1 to 5, 

by appending modifier 59 if supported by the documentation. This is supported with the CCM indicator 1. The [[modifier]] is added to the column 2 code (in this case code 11720).

##### Example 3
>11042, Debridement, subcutaneous tissue (includes epidermis and dermis, if performed); first 20 square cm or less 

and 

>11001, Debridement of extensive eczematous or infected skin; each additional 10% of the body surface 

have an indicator of 9. This indicator means that an NCCI [[edit]] does not apply.

```ad-billing
title: Billing
When a payer denies a procedure or service as inclusive to (or included in) another procedure, first review the bundling edits to see if these two procedures are bundled. If a [[modifier]] is allowed, separate the two procedures and make sure documentation is available to support the billing of both procedures. Many payers utilize the NCCI edits and add their own edits to the NCCI edits. The provider’s contract with the insurance payer may also stipulate bundling edits.
```

### [[Modifiers]] and NCCI Edits
[[HCPCS Level II]] or [[Current Procedural Terminology|CPT]]® [[modifiers]] may be used to bypass the NCCI edits in certain circumstances when appropriate. It is important as a biller to understand [[modifier]] usage. This allows for proper appeals to be filed when warranted and to understand when a [[write-off]] should be done instead. The reimbursement process will be delayed if an appropriate [[modifier]] was warranted but not appended. Not understanding correct [[modifier]] usage will cause an initial denial and require extra work to rebill and receive appropriate payment.

#### Eligible NCCI [[Modifiers]]
The [[modifiers]] that may be used to bypass the NCCI edits include:
- Anatomic [[modifiers]]: E1-E4, FA, F1-F9, TA, T1-T9, LT, RT, LC, LD, RC, LM, RI
	- E1-E4: describe upper and lower, right and left eyelids (different anatomic sites)
	- FA, F1-F9 describe left and right hands, and specific fingers of each (different anatomic sites)
	- TA, T1-T9 describe left and right foot with each specific toe of each (different anatomic sites)
- Global surgery [[modifiers]]: 24, 25, 57, 58, 78, 79
- Other [[modifiers]]: 27, 59, 91, XE, XS, XP, XU

#### Ineligible NCCI [[Modifiers]]
[[Modifiers]] 76 Repeat procedure or service by same physician or other qualified healthcare professional, and 77 Repeat procedure or service by another physician or other qualified healthcare professional are not NCCI [[edit]] [[modifiers]] and cannot be used to bypass edits.

### [[Medicaid]] and NCCI
As stated earlier, the [[Patient Protection and Affordable Care Act|ACA]] requires [[Medicaid]] to utilize the NCCI edits. [[CMS]] allows states to deactivate edits that conflict with state laws, regulations, administrative rules, payment policies, and/or level of operational readiness. The Medicaid NCCI edits apply only to Medicaid fee-for-service claims reimbursed for [[HCPCS Level II|HCPCS]]/[[Current Procedural Terminology|CPT]]® codes.

#### Methodologies
The [[Medicaid]] NCCI program consists of six methodologies:
1. A methodology with Procedure-to-Procedure (PTP) edits for practitioner and ambulatory surgical center (ASC) services
2. A methodology with PTP edits outpatient hospital services
3. A methodology with PTP edits for durable medical equipment
4. A methodology with [[Medically Unlikely Edits|MUEs]] for practitioner and ASC services
5. A methodology with [[Medically Unlikely Edits|MUEs]] for outpatient hospital services for hospitals
6. A methodology with [[Medically Unlikely Edits|MUEs]] for durable medical equipment

Each of the [[Medicaid]] NCCI methodologies has four components:
1. A set of edits
2. Definitions of types of [[Claim Form|claims]] subject to the edits
3. A set of claim [[adjudication]] rules for applying the edits
4. A set of rules for addressing provider appeals of denied payments for services based on the edits

## Resources for NCCI Edits
[HCPCS - General Information | CMS](https://www.cms.gov/Medicare/Coding/MedHCPCSGenInfo/index.html)
Provides background information, coding updates and transmittals, and coding process and criteria information for the Healthcare Common Procedure Coding System (HCPCS) code set.

**Internet-Only Manual (IOM) Pub 100-04 - Medicare Claims Processing Manual**
[https://www.cms.gov/Regulations-and-Guidance/Guidance/Manuals/downloads/clm104c23.pdf](https://www.cms.gov/Regulations-and-Guidance/Guidance/Manuals/downloads/clm104c23.pdf)
Chapter 23 is entitled “[[Fee Schedule]] Administration and Coding Requirements.” Section 20.9, “Correct Coding Initiative (CCI),” provides instructions regarding implementation of NCCI edits and [[Medically Unlikely Edits|MUEs]] including information on [[modifiers]].

**Medicare Claim Review Programs**
[https://www.cms.gov/Research-Statistics-Data-and-Systems/Monitoring-Programs/Medicare-FFS-Compliance-Programs/Medical-Review/index.html](https://www.cms.gov/Research-Statistics-Data-and-Systems/Monitoring-Programs/Medicare-FFS-Compliance-Programs/Medical-Review/index.html)
[https://www.cms.gov/Regulations-and-Guidance/Guidance/Manuals/Downloads/pim83c01.pdf](https://www.cms.gov/Regulations-and-Guidance/Guidance/Manuals/Downloads/pim83c01.pdf)
[https://www.cms.gov/Regulations-and-Guidance/Guidance/Manuals/Downloads/pim83c03.pdf](https://www.cms.gov/Regulations-and-Guidance/Guidance/Manuals/Downloads/pim83c03.pdf)

**The National Correct Coding Initiative in Medicaid**
[Medicaid NCCI Edit Files | Medicaid](https://www.medicaid.gov/medicaid/program-integrity/ncci/edit-files/index.html)
The [[CMS]] National Correct Coding Initiative (NCCI) promotes national correct coding methodologies and reduces improper coding, which may result in inappropriate payments of [[Medicare]] Part B claims and [[Medicaid]] claims. The [[Medicaid]] NCCI program has significant differences from the [[Medicare]] NCCI program. The National Correct Coding Initiative in Medicaid webpage provides information and resources about NCCI policies under the [[Medicaid]] program.

**National Correct Coding Initiative Policy Manual for Medicare Services**
[National Correct Coding Initiative Edits | CMS](https://www.cms.gov/Medicare/Coding/NationalCorrectCodInitEd/index.html)
The manual is available in the Downloads section at the bottom of the National Correct Coding Initiative Edits page on the CMS website. The manual serves as a reference tool for correct coding and to explain the rationale for NCCI edits.

**Quarterly Provider Updates**
CMS Quarterly Provider Updates can be located at:
[CMS.gov](https://www.cms.gov/Regulations-and-Guidance/Regulationsand-Policies/QuarterlyProviderUpdates/index.html)
CMS offers a free email subscription service, which provides notifications electronically when new information is available.

[Centers for Medicare & Medicaid Services (CMS)](https://public.govdelivery.com/accounts/USCMS/subscriber/new?topic_id=USCMS_11966)
The Quarterly Provider Updates electronic mailing list notifies subscribers via email immediately of any regulations or program instructions released during the quarter that affect Medicare providers, including transmittals of the quarterly updates to the NCCI.

**Quarterly PTP and MUE Version Update Changes**
[Quarterly PTP and MUE Version Update Changes | CMS](https://www.cms.gov/Medicare/Coding/NationalCorrectCodInitEd/Version_Update_Changes.html)
Quarterly changes to the Column 1/Column 2 and MUE tables can be found on the Quarterly PTP and [[Medically Unlikely Edits|MUE]] Version Update Changes webpage.

**Change Request 8853**
[https://www.cms.gov/Regulations-and-Guidance/Guidance/Transmittals/Downloads/R1421OTN.pdf](https://www.cms.gov/Regulations-and-Guidance/Guidance/Transmittals/Downloads/R1421OTN.pdf)
Change Request 8853 provides information about [[Medically Unlikely Edits]] (MUEs) and the MUE [[Adjudication]] Indicator (MAI).