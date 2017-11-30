- Speaker Rich Alberth
- The following tools are used for scanning AWS environment.
  - SurveyMonkey
  - Nessus "Caffeine" Application
  - Redhat Openscap
- Athena is a distributed, serverless, SQL Engine with S3 backend
- It allows to ask complicated questions about data in S3 objects
- S3 objects directly participate in other "big data" systems
- Helps query your flow log and audit trail
- Athena uses Hive & Presto under the covers
- Table 'census_facts' is all S3 files with prefix 'census/facts/'
- RegEx Format ROW FORMAT SERDE
```
^([^[]+)\[[([A-Z]+)\]
```
- Columnar Files
  - 2 Formats - Park, ORC
  - 3 Rules   - Group Columns, Metadata, Lots of Pointers
