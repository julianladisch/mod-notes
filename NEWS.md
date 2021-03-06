## 2.1.0 2018-06-06
 * MODNOTES-31 "readonly" fields like creatorUserName, etc should be ignorable
 * MODNOTES-34 Update the 'domain-models-runtime' dependency version
 * MODNOTES-37 GET /notes/_self requires unexpected permission
 * MODNOTES-15 Query validation
 * MODNOTES-39 Fix invalid UUIDs
 * general tightening of error responses, using RMB's helpers where possible
 * Code cleanup

## 2.0.1 2017-11-14
 * MODNOTES-24 Upgrade to RMB 15
 * Requires interface 'users' in 14.0 or 15.0
 * MODNOTES-29 /notes endpoint accepts arbitrary key-value pairs
 * MODNOTES-30 Add "populateJsonWithId" to the db-schema json file

## 2.0.0 2017-10-20
 * MODNOTES-19: parse tags and trigger notifications to users mentioned
 * MODNOTES-16: More granular permissions for domains
 * MODNOTES-18: include user full name
 * MODNOTES-23: PUT request wipes out creator details

Breaking changes:
 * Much stricter permissions, need to have notes.domain.XXX, matching the domain
of the notes you operate on (for example, notes.domain.users).
 * PUT request validates that the creatorUserName and creatorLastName are required.
(not so in POST, they get looked up).
 * New dependencies: mod-users and mod-notify

## 1.0.1
 * FOLIO-834

## 1.0.0
 * 'metaData' renamed to 'metadata', due to RMB 14.0.0. This is a BREAKING CHANGE!
   Changes the way records are returned, and what queries are accepted.
 * MODNOTES-13 Execute a git submodule init/update in mvn install
 * More test cases

## 0.2.0
 * MODNOTES-2: Metadata section
 * MODNOTES-3: Unit tests
 * MODNOTES-7: Implement the `_self` endpoint
 * MODNOTES-9: Permissions in the ModuleDescriptor
 * MODNOTES-10: totalRecords instead of total_records

## 0.1.1
* Docker image

## 0.1.0
* Initial implementation: basic CRUD operations in place

