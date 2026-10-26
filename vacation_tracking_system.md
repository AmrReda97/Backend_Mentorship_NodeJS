# 1. Problem Definition

Workers can work on multiple projects and with multiple managers. As a result, managers and workers need a way to manage and keep track of the vacation time of workers and themselves as well.

In the past, all vacation time had to be approved by an immediate manager and then checked by a clerk in the HR department before it was authorized. Sometimes this manual process could take days.

# 2. Vision

A Vacation Tracking System (VTS) will provide individual employees with the capability to manage their own vacation time, sick leave, and personal time off, without having to be an expert in company policy or the local facility’s leave policies.

The main goal of this application is to improve the internal business processes of this organization, at least with respect to the time it takes to manage vacation time requests.

An automated system will speed up this process and will require at most one manual approval by the immediate manager (some high-level employees may not require manager approval).

# 3. Actors

1. **Employee:** The main user of this system. An employee uses this system to manage his or her vacation time.
2. **Manager:** An employee who has all the abilities and goals of a regular employee, but with the added responsibility of approving vacation requests for immediate subordinates. A manager may award subordinates comp time, subject to certain limits set in the system.
3. **Clerk:** A member of the HR department who has sufficient rights to view employees’ personal data and is responsible for ensuring that employees’ information in all HR systems is up to date and correct. An HR clerk can add or remove nearly any record in the system. In the real world, HR clerks may or may not be employees; however, if they are employees, they use two separate login IDs to manage these two different roles.
4. **System Admin:** A role responsible for the smooth running of the system’s technical resources (e.g., Web server, database) and for collecting and archiving all log files.

# 4. Requirements

## 4.1. Functional Requirements

- The system allows all kinds of employees to validate and verify leave/vacation time requests.
- Allows managers to approve/disapprove leave/vacation time requests.
- Provides access to requests for the previous calendar year and allows requests to be made up to a year and a half in the future.
- Sends e-mail notifications to request manager approval and notify employees of request status changes.
- Keeps activity logs for all transactions.
- Enables HR and system administration personnel to override all actions restricted by rules, with logging of those overrides.
- Allows managers to directly award personal leave time (with system-set limits).
- Provides a Web service interface for other internal systems to query any given employee’s vacation request summary.
- Provides interfaces with the HR department’s legacy systems to retrieve required employee information and changes.

## 4.2. Non-Functional Requirements

- The system should be easy to use for all kinds of actors.

## 4.3. Constraints

- Uses existing hardware and middleware.
- Is implemented as an extension to the existing intranet portal system and uses the portal’s single-sign-on mechanisms for all authentication.
- The system should be built as a Web-centric application.
