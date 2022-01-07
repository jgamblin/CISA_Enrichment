# CISA Known Exploited Vulnerabilities Catalog Enrichment

The [CISA](https://www.cisa.gov/) recently started to publish the [Known Exploited Vulnerabilities Catalog Enrichment](https://www.cisa.gov/known-exploited-vulnerabilities-catalog) to help federal agencies keep up with exploited vulnerabilities.

The data they provide is minimal, so I have built this jupyter notebook to enrich the data using the [CIRCL](https://circl.lu/) public [CVE API](https://www.circl.lu/services/cve-search/#cve-search-common-vulnerabilities-and-exposure-web-interface-and-api) to add the following data points:

- CWE
- CVE Published Date
- CVE Modified Date
- Reference URLs
- CPE 2.3 Data

A Github Action runs every 6 hours and updates the following files:

- [cisa_enriched.csv](cisa_enriched.csv)
- [cisa_enriched.json](cisa_enriched.json)
