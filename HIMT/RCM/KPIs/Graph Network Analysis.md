# Graph Network Analysis
## Referring Providers to Rendering Providers
### Referral Pattern Analysis Methodology (Moore)
Savvy practices can use data outside of their PM systems to analyze patient referral patterns. One source of data to consider is that provided by [[CMS]]. In response to a Freedom of Information Act request, CMS released data relating to providers who provide services to common patients. If two providers bill services to the same patient within 30, 60, 90, or 180 days, those two providers’ NPI numbers are linked in the data. The data assumes a shared relationship between the first provider and the second provider if the two providers submit claims for the same patient within those four date intervals.

#### The data shows five columns:
1. First NPI to render services
2. Second NPI to render services
3. Number of visits
4. Number of unique common patients
5. Number of patients treated on the same day

>==**Table 1. Example of Presumed Shared Relationship Data**==

| FromNPI    | ToNPI      | Referrals | Beneficiaries | SameDay |
| ---------- | ---------- | --------- | ------------- | ------- |
| 1000000004 | 1548295421 | 25        | 11            | 8       |
| 1000000004 | 1790775229 | 60        | 22            | 30      |
| 1000026017 | 1598773715 | 35        | 15            | 18      |
| 1003000126 | 1003888777 | 32        | 12            | 0       |
| 1003000126 | 1003951625 | 147       | 78            | 27      |
| 1003000126 | 1003975400 | 51        | 28            | 1       |
| 1003000126 | 1013051119 | 24        | 15            | 1       |
| 1003000126 | 1013902600 | 45        | 25            | 3       |
| 1003000126 | 1023027109 | 29        | 21            | 3       |
| 1003000126 | 1023029964 | 42        | 23            | 0       |
| 1003000126 | 1033187000 | 119       | 34            | 2       |
| 1003000126 | 1033469317 | 33        | 19            | 3       |
| 1003000126 | 1043265804 | 68        | 26            | 34      |
| 1003000126 | 1053306746 | 94        | 47            | 41      |

The trick is to use the CMS data as a proxy for patient referrals. For example, if 45 patients saw Provider A and then saw Provider B, there is a good chance that at least some of those 45 patients were referred by Provider A. By carefully analyzing the referral proxy data, practices can get an estimate of their share of referrals in a given market. Using the same example, if Provider A also had a relationship with Provider C that shared 90 patients, Provider B could estimate that she is getting about one-third (45 / (45 + 90)) of the patients referred by Provider A. Table 2 groups all referrals to a practice in one column and referrals outside a practice separately in a pivot table analyzing the CMS data.

>==**Table 2. Grouped Referrals: Referred Patients vs. Not Referred**==

| [[Referring Provider]] | No. Referred | No. NOT Referred | Percentage |
| ------------------ | ------------ | ---------------- | ---------- |
| Espino, Joey       | 437          | 219              | 66.6%      |
| Petrillo, Eugene   | 418          | 0                | 100.0%     |
| Marciniak, Shayne  | 407          | 520              | 13.9%      |
| Dash, Robert       | 365          | 385              | 48.7%      |
| Gunther, Micah     | 332          | 277              | 54.5%      |
| Disanto, Carletta  | 286          | 211              | 57.5%      |
| Handy, Berta       | 261          | 130              | 66.8%      |
| Rimer, Sharyn      | 245          | 234              | 51.1%      |
| Fields, Grisel     | 237          | 261              | 47.6%      |
| Dimauro, Rueben    | 233          | 134              | 63.5%      |
| Loveland, Laura    | 223          | 114              | 66.2%      |
| Dull, Janee        | 213          | 281              | 43.1%      |
| Mayne, Francesca   | 204          | 109              | 65.2%      |
| Mclendon, Ruthanne | 201          | 76               | 72.6%      |

There are some issues to be aware of when using the CMS data. Though CMS releases four sets of data based on the interval between Providers A and B, the 30-day data tends to have the least amount of noise in it. The longer the time between seeing Provider A and seeing Provider B, the higher the odds that something besides a referral is driving the shared patient relationship.

CMS considers a wide range of providers when creating this data. Ambulances and labs are very commonly added. To give some feel for the scope of this, the 2014 full-year data with a 30-day shared interval is over 138 million rows. To even download that much data takes a tool much more powerful than Excel. SQL Server is the typical way to go, but specialized statistical software packages are also used. Once the data is downloaded, practices may find they can look for specific NPIs in the data. One approach would be to identify an important referral source to search for as the first provider in the data. Then, look for referral patterns from that source. Since the CMS data only includes NPI numbers, it is helpful to download an NPI database and cross-reference the NPIs. The NPI data will include a business mailling address and one practice address. Having only one address limits the ability to map data to see where referrals are coming from when providers practice at more than one location. The NPI data also includes multiple taxonomy codes which can be used to estimate provider specialties.

Using the taxonomy codes and a practice’s general knowledge of their market helps filter out providers that are unlikely sources of referrals. By applying several levels of filtering, the massive amount of CMS data available can be made more manageable and thereby more useful.

Another complication with the NPI numbers is that the CMS data reflects how the claim was billed. If the claim was billed under a different NPI than the practice is expecting, the data may not reflect the underlying referral patterns. If the NPI relates to a group or organization instead of an individual provider, it can be more difficult to determine the sources of referrals or how many referrals a provider might be making to competing practices.

CMS has also filtered the data to protect patient privacy. Relationships between Provider A and B with fewer than 11 unique beneficiaries are excluded from the data. If a referral source has a shared relationship with 8 providers in a group practice and the referral source sends 10 [[Medicare]] beneficiaries to each provider, none of the 80 beneficiaries will be included in the data. Major potential sources of referrals can be masked by the fewer than 11 beneficiaries rule.

Even with these caveats, the CMS data can give practices unparalleled insight into referral patterns. The data can also estimate a practice’s market share of referrals from major providers.

# Flourish Example
<iframe src='https://flo.uri.sh/visualisation/7383404/embed' title='Interactive or visual content' class='flourish-embed-iframe' frameborder='0' scrolling='no' style='width:100%;height:600px;' sandbox='allow-same-origin allow-forms allow-scripts allow-downloads allow-popups allow-popups-to-escape-sandbox allow-top-navigation-by-user-activation'></iframe><div style='width:100%!;margin-top:4px!important;text-align:right!important;'><a class='flourish-credit' href='https://public.flourish.studio/visualisation/7383404/?utm_source=embed&utm_campaign=visualisation/7383404' target='_top' style='text-decoration:none!important'><img alt='Made with Flourish' src='https://public.flourish.studio/resources/made_with_flourish.svg' style='width:105px!important;height:16px!important;border:none!important;margin:0!important;'> </a></div>

# Links
- [Referral Data FAQs | CMS](https://www.cms.gov/Regulations-and-Guidance/Legislation/FOIA/Referral-Data-FAQs)
- [Data on the Open Data Network](https://www.opendatanetwork.com/search?categories=health&ref=hp)
- [FOIA - Publicly Available Information Index](https://www.cms.gov/center/freedom-of-information-act/index.html)
- [Find, Request and Use CMS Data | ResDAC](https://resdac.org/)
- [Relationships between physicians and Pharma](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC5765617/)
- [Open Payments Data - CMS](https://openpaymentsdata.cms.gov/dataset/29v2-guh5)
- [Dollars for Docs - ProPublica](https://projects.propublica.org/docdollars/)
- [Exclusions | Office of Inspector General | U.S. Department of Health and Human Services](https://oig.hhs.gov/exclusions/index.asp)
- [The NPDB - Public Use Data File](https://www.npdb.hrsa.gov/resources/publicData.jsp)