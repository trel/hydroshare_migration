# hydroshare_migration

irods version 4.2.11

## setup

- two zones at RENCI - data zone and user zone
- two zones at GCP - data zone and user zone
- rename GCP data zone - new name TBD...
  - update client(s)
  - update Django app
  - update GCP user zone (already federated)
- confirm GCP zones behaving as expected/desired
- federate RENCI data zone with renamed GCP data zone
- confirm connectivity with small and large files
- update GCP Django app with new zone name

## syncing

- write rule/PEP for irsync from RENCI to GCP when updates happen in RENCI
- add delay to this rule
- test rules in docker-compose.yml federation

## migration

- declare maintenance window
- confirm sync is up-to-date
- open maintenance window
- migrate Django app
- turn on Django app
- switch DNS?

## conformance testing

- confirm monitoring and logging all functional
- run tests to determine sufficient success
- close maintenance window

