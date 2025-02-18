# Requirements Traceability Matrix (RTM)

This RTM maps the key business requirements for the "Managing Performance Rating and Award" workflow to their associated test cases. It ensures full coverage of functionality—from form submissions and approvals to conditional logic and email notifications.

| Requirement ID | Business Requirement Description | Test Case(s) | Comments |
|---------------|--------------------------------|--------------|----------|
| RQ-001 | Supervisor assigns and selects the appropriate performance rating plan cover sheet. | TC-001, TC-002 | Covers manual validation of supervisor actions in form assignment. |
| RQ-002 | Director reviews and approves the performance rating plan cover sheet. | TC-003, TC-004 | Verifies proper routing and approval of the cover sheet by the director. |
| RQ-003 | If the Director disapproves (with reason), the cover sheet returns to the Supervisor for corrections. | TC-005, TC-006 | Ensures the rejection path is handled and correction cycles are initiated. |
| RQ-004 | After corrections, the Director re-approves the cover sheet. | TC-007 | Validates the re-submission and re-approval process. |
| RQ-005 | Examiner receives an email notification to sign the cover sheet; if the Examiner does not sign, the Supervisor can bypass with a reason. | TC-008, TC-009 | Tests both the email notification trigger and the bypass functionality. |
| RQ-006 | Supervisor initiates the midyear rating process, optionally adding review comments before submission. | TC-010, TC-011 | Confirms midyear rating initiation and supervisor review options. |
| RQ-007 | Director reviews the midyear rating; if disapproved, the form is returned for corrections. | TC-012, TC-013 | Validates the midyear rating review cycle, including rejection and correction handling. |
| RQ-008 | Examiner reviews the midyear rating and signs, or the Supervisor bypasses if the Examiner does not sign. | TC-014, TC-015 | Ensures proper handling of the midyear examiner sign-off and bypass process. |
| RQ-009 | Supervisor enters end‑of‑year rating points and submits the form for Director review. | TC-016, TC-017 | Verifies the entry of rating points and the submission process. |
| RQ-010 | Director reviews the end‑of‑year rating; if rejected (with a reason), it is returned for corrections. | TC-018, TC-019 | Confirms the review cycle for end‑of‑year ratings, including the rejection and correction process. |
| RQ-011 | Examiner signs the end‑of‑year rating, or the Supervisor bypasses with a reason if the Examiner does not sign. | TC-020, TC-021 | Validates the final sign-off process and the bypass option for end‑of‑year ratings. |
| RQ-012 | The system applies a probation rating for employees with less than one year of service. | TC-022 | Ensures the conditional logic correctly assigns a probation rating. |
| RQ-013 | For employees who have changed positions and whose performance rating plan started before June 2nd, the midyear and end‑of‑year rating processes are applied; otherwise, a probation rating is used. | TC-023, TC-024 | Checks conditional logic based on position change and start date conditions. |
| RQ-014 | The system sends email notifications at each key transition (e.g., Director approval, Examiner notification). | TC-025, TC-026 | Validates that email notifications are triggered and contain accurate information. |


This RTM serves as a dynamic tool during testing to ensure that every business requirement is met by one or more test cases.
