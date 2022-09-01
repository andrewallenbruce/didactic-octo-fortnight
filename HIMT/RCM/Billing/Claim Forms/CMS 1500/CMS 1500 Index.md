---
title: CMS 1500 Index
author: Andrew Bruce
tags: CMS1500, HCFA, claimsform
---
# General Instructions
## Punctuation
### Names
Commas are used to separate the last name, first name, and middle initial. A hyphen can be used for hyphenated names. Do not use periods within the name.
### Address
Do not use punctuation or other symbols in the address. For example, a 9-digit ZIP code is entered without the hyphen. One of the top 10 reasons electronic claims are rejected is due to an invalid ZIP code.
### Dates
Providers and suppliers must report 8-digit dates in all date of birth fields (items 3, 9b, and 11a), and either 6-digit or 8-digit dates in all other date fields (items 11b, 12, 14, 16, 18, 19, 24a, and 31).
- Providers and suppliers have the option of entering either a 6 or 8-digit date in items 11b, 14, 16, 18, 19, or 24a. 
	- However, if a provider of service or supplier chooses to enter 8-digit dates for items 11b, 14, 16, 18, 19, or 24a, he or she must enter 8-digit dates for all these fields. For instance, a provider of service or supplier will not be permitted to enter 8-digit dates for items 11b, 14, 16, 18, 19 and a 6-digit date for item 24a. 
- The same applies to providers of service and suppliers who choose to submit 6-digit dates too. Items 12 and 31 are exempt from this requirement.
# Items
### [[CMS 1500 Item 1]]
### [[CMS 1500 Item 1a]]
### [[CMS 1500 Item 2]]
### [[CMS 1500 Item 3]]

- **Item 5**: Enter the patient’s mailing address and telephone number. On the first line enter the street address; the second line, the city and state; the third line, the ZIP code and phone number. This information is provided by the patient and confirmed with the photo ID. Remember: Punctuation is not used in the address. It is recommended that a phone number not be reported unless required by the carrier (for example, Workers’ Compensation or Property and Casualty claims). The phone number is not transmitted in the electronic 837 file. The address used is the patient’s permanent address. If the patient has a temporary address, such as a college student away for school, the temporary address is not reported.

- **Item 6**: Check the appropriate box for patient’s relationship to insured when item 4 is completed. This question is asked during the registration process and stored in the practice management system.

- **Item 7**: Enter the insured’s address and telephone number (the telephone number is only completed when required by the payer). When the address is the same as the patient’s, enter the word *SAME*. Complete this item only when items 4, 6, and 11 are completed. Complete this item only when item 4 is completed. It is recommended that a phone number not be reported unless required by the carrier (for example, Workers’ Compensation or Property and Casualty Claims). The phone number is not transmitted in the electronic 837 file. For Workers’ Compensation claims, the address of the employer is reported.

- **Item 8**: *Leave blank. This field is reserved for NUCC use.*

- **Item 9**: Enter the last name, first name, and middle initial of the insured if the patient has a secondary insurance. This is completed if **Item 11d** is marked YES. Medigap: Complete this information if the patient has a Medigap (Medicare supplemental insurance) policy and the insured’s name is different from that shown in item 2. Otherwise, enter the word SAME. If no Medigap benefits are assigned, leave blank. NOTE: Only participating physicians and suppliers are to complete item 9 and its subdivisions and only when the beneficiary wishes to assign his or her benefits under a MEDIGAP policy to the participating physician or supplier.

- **Item 9a**: Enter the policy and/or group number of the secondary insurance. (for example, Medigap policy number preceded by MEDIGAP, MG, or MGAP). NOTE: Item 9d must be completed, even when the provider enters a policy and/or group number in item 9a.

- **Item 9b**: *Leave blank. This field is reserved for NUCC use.*

- **Item 9c:** *Leave blank if Item 9d is completed. This field is reserved for NUCC use.*

- **Item 9d**: Enter the other insured’s insurance plan or program name. Medigap: Enter the 5-digit Coordination of Benefits Agreement (COBA) Medigap-based Identifier (ID).

- **Items 10a through 10c**: Check YES or NO to indicate whether employment, auto liability, or other accident involvement applies to one or more of the services described in item 24. Enter the state postal code. Any item checked YES indicates there may be other insurance primary to the patient’s health insurance. For example, if the encounter was to treat a patient’s injury while at work, workers’ compensation is the primary payer not the patient’s health insurance. Identify primary insurance information in item 11.

- **Item 10d**: Claim codes are entered in this item to identify additional information about the patient’s condition on the claim. Current claim codes include condition codes. Condition codes approved for use in this item include codes for abortions, sterilization, and codes for workers’ compensation claims. Condition codes are not used when submitting a revised or corrected claim. Examples of workers’ compensation condition codes are:

			- W2 Duplicate of original bill
			- W3 Level 1 appeal
			- W4 Level 2 appeal
			- W5 Level 3 appeal

- **Item 11**: This item contains the insured’s policy, group, or FECA number (9-character identifier assigned to a patient claiming work-related condition(s) under the Federal Employees Compensation Act 5 USC 8101) as it appears on the insured’s healthcare identification card. Do not use a hyphen or space as a separator within the policy or group number. If item 4 is completed, this item must also be completed. Medicare: This item is required by Medicare. By completing this item, the physician/supplier acknowledges having made a good faith effort to determine whether Medicare is primary or secondary payer. If there is insurance primary to Medicare, enter the insured’s policy or group number and proceed to items 11a–11c. This is determined by having the patient complete the Medicare Secondary Questionnaire. Items 4, 6, and 7 must also be completed. NOTE: Enter the appropriate information in item 11c if insurance primary to Medicare is indicated in item 11. If there is no insurance primary to Medicare, enter the word NONE and proceed to item 12. If the insured reports a terminating event with regard to insurance which was primary to Medicare (for example, insured retired), enter the word NONE and proceed to item 11b.

- **Item 11a**: Enter the insured’s 8-digit birth date (MM|DD|CCYY) and sex. If the gender is unknown, leave it blank.

- **Item 11b**: Enter a qualifier (for example, Y4 Property Casualty Claim Number) followed by the identifier number. For Medicare, enter employer’s name. If there is a change in the insured’s insurance status (for example, retired), enter either a 6-digit (MM|DD|YY) or 8-digit (MM|DD|CCYY) retirement date preceded by the word RETIRED. This information should be entered to the right of the vertical dotted line.

- **Item 11c**: Enter the name of the insurance plan or program of the insured. Medicare: Enter the 9-digit PAYERID number of the primary insurer. If no PAYERID number exists, then enter the complete primary payer’s program or plan name. If the primary payer’s explanation of benefits (EOB) does not contain the claims processing address, record the primary payer’s claims processing address directly on the EOB. This is required if there is insurance primary to Medicare that is indicated in item 11.

```ad-billing
title: Billing Tip
Some insurers require an identification number of the primary insurer rather than the name in this field.
```

- **Item 11d**: This is marked to indicate if the patient has secondary insurance. If this item is marked, items 9, 9a, and 9d must also be completed. Medicare: Leave blank. It is not required.

```ad-billing
title: Billing Tip
If the patient has a primary and secondary insurance, the secondary insurer will not pay the claim until the primary insurance has decided. For Medicare, if the patient has a secondary insurance on file, Medicare will cross the claim over to the secondary payer once Medicare has made a payment determination (paid or denied). For payers that do not cross claims over, once the EOB is received from the primary insurance apply the payment or denial and submit a claim and copy of the primary insurance EOB to the secondary payer for consideration.
```

- **Item 12**: The patient or authorized representative must sign and enter either a 6-digit date (MM|DD|YY), 8-digit date (MM|DD|CCYY), or an alpha-numeric date (for example, January 1, 2016) unless the signature is on file. In lieu of signing the claim form, the patient may sign a statement to be retained by the provider, physician, or supplier. This form is signed by the patient when completing new patient paperwork or updating paperwork. 

	NOTE: This can be Signature on File, SOF, or a computer generated signature. A date is only entered when a legal signature is used. The patient’s signature authorizes release of medical information necessary to process the claim. It also authorizes payment of benefits to the provider of service or supplier when the provider of service or supplier accepts assignment on the claim. 
	
	Accepting assignment means the provider bills the patient’s insurance and receives payment directly from the patient’s insurance. By accepting assignment, the provider or facility agrees to the payer’s fee schedule.

- **Item 13**: The patient’s signature or the statement Signature on File, or SOF in this item authorizes payment of medical benefits to the physician or supplier. The patient or his/her authorized representative signs this item or the signature must be on file separately with the provider as an authorization.

- **Item 14**: Enter either an 8-digit (MM|DD|CCYY) or 6-digit (MM|DD|YY) date of current illness, injury, or pregnancy (LMP). Enter the applicable qualifier to the right of the vertical dotted line to identify which date is being reported. Qualifiers include:

				- 431 Onset of Current Symptoms or Illness
				- 484 Last Menstrual Period

	Medicare: Medicare does not use the qualifier information. Do not enter a qualifier for Medicare claims.

```ad-billing
title: Billing Tip
Medicare commonly rejects claims for an invalid future date within the Onset, Acute Manifestation, Initial Treatment, Accident, or Last Menstrual Period date fields.
```

- **Item 15**: Enter another date related to the patient’s condition or treatment in either an 8-digit (MM|DD|CCYY) or a 6-digit (MM|DD|YY) format. Check with your payers to determine if this item needs to be completed. For Medicare: Leave blank. This item is not required. Enter the applicable qualifier to identify which date is being reported:

				- 454 Initial Treatment
				- 304 Latest Visit or Consultation
				- 453 Acute Manifestation of a Chronic Condition
				- 439 Accident
				- 455 Last X-ray
				- 471 Prescription
				- 090 Report Start (Assumed Care Date)
				- 091 Report End (Relinquished Care Date)
				- 444 First Visit or Consultation

- **Item 16**: If the patient is employed and unable to work in his or her current occupation, enter an 8-digit (MM|DD|CCYY) or 6-digit (MM|DD|YY) date of when patient is unable to work. An entry in this item may indicate employment related insurance coverage. If the patient is treated for a work-related injury, the claim is submitted to workers’ compensation not the patient’s medical insurance.

- **Item 17**: Enter the name of the referring or ordering physician if the service or item was ordered or referred by a physician. The name should be entered as First Name, Middle Initial, Last Name, followed by the provider’s credentials. Do not use commas or periods. A hyphen can be used for a hyphenated name. In addition to the information above, the supervising physician can also be reported in this field. When multiple providers are involved, enter one provider using the following priority order:

		- 1. Referring Provider (Qualifier DN)
		- 2. Ordering Provider (Qualifier DK)
		- 3. Supervising Provider (Qualifier DQ)

	Enter the applicable qualifier to the left of the vertical dotted line. Medicare: All physicians who order services or refer Medicare beneficiaries must report this data. When more than one provider is involved, use a separate CMS-1500 claim form for each referring, ordering, or supervising physician.

- Item 17a: Enter the Other ID number of the referring, ordering, or supervising  provider. Enter the qualifier to indicate what number is being reported:
0B State License Number
1G Provider UPIN Number
G2 Provider Commercial Number
LU Location Number (used for the supervising provider
only)
Medicare: Leave blank.
Item 17b—Enter the National Provider Identifier (NPI) of
the referring/ordering/supervising physician or non-physician
practitioner listed in item 17. NPIs are required for all
providers and facilities. Application for NPIs can be submitted
online through the CMS website.
Item 18—Enter either an 8-digit (MM|DD|CCYY) or a 6-digit
(MM|DD|YY) date when a medical service is furnished as a
result of, or subsequent to, a related hospitalization.
Item 19—Payers have different uses for this item. For example,
enter the drug’s name and dosage when submitting a claim for
Not Otherwise Classified (NOC) drugs. NOC means the code
is unspecified and the code alone will not adequately report the
drug administered. The drug administered needs to be identified
for the payer to determine proper reimbursement.
In addition to the information above, report the appropriate
qualifier to describe the identifier. Qualifiers can be found in
the NUCC claim form manual and include general qualifiers
and Workers’ Compensation qualifiers for the report type and
transmission type.
When modifier 99 (multiple modifiers) is entered in item 24d,
enter all applicable modifiers. If modifier 99 is entered on
multiple line items of a single claim form, all applicable modifiers
for each line item containing a 99 modifier should be
listed as follows: 1= (mod), where the number 1 represents the
line item and “mod” represents all modifiers applicable to the
referenced line item.