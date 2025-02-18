# Master Test Plan

## Project: Managing Performance Rating and Award  
**Version:** 1.0  
**Prepared By:** [Your Name]  
**Date:** [Insert Date]  

## 1. Introduction

### Purpose:
This Master Test Plan defines the testing strategy, objectives, and execution approach for the "Managing Performance Rating and Award" workflow. The goal is to validate the complete end-to-end process—from the initial performance rating plan cover sheet through midyear and end‑of‑year rating cycles, ensuring correct routing, approval, and exception handling.

### Background:
The application automates performance rating workflows where forms are submitted, reviewed, and approved by the supervisor, director, and examiner (with a supervisor bypass option for examiner signature). The process differentiates between probation, midyear, and end‑of‑year ratings based on employee tenure and position change conditions. Note that:

- New hire employee tests are not included in this flow.
- For employees who have changed positions, combined rating scenarios will not be addressed in this cycle.

## 2. Objectives

### Primary Objectives:
- Validate the complete functional workflow of the performance rating process.
- Ensure that the conditional logic (e.g., employee tenure, position change, and cutoff dates) behaves as expected.
- Verify that email notifications and approval cycles (including re-submission on disapproval) function correctly.

### Secondary Objectives:
- Identify and document any defects or integration issues.
- Establish a robust baseline for both manual and automated testing.
- Prepare a reusable set of test cases for future regression cycles.

## 3. Scope

### In-Scope:
#### **Performance Rating Plan Cover Sheet Process:**
- Supervisor assigns the form and selects the appropriate cover sheet.
- Director reviews the form; if disapproved, it is sent back for correction.
- Final approvals are completed by both supervisor and director.
- Examiner receives the email notification and either signs or is bypassed by the supervisor (with a reason).

#### **Midyear Rating Process:**
- Supervisor optionally adds a review, signs, and approves the midyear rating form.
- Director review, with re-submission for corrections on disapproval.
- Examiner review with the possibility of bypass.

#### **End‑of‑Year Rating Process:**
- Supervisor inputs rating points, sends the form to the director.
- Handling of director disapproval with corrections and re-submission.
- Final examiner sign-off or supervisor bypass.

#### **Tools and Test Artifacts:**
- Manual test cases maintained in Rally Agile.
- Automation test scripts developed using Selenium Serenity Cucumber.
- Use of a dedicated test environment and test database.

### Out-of-Scope:
- Employee new hire testing scenarios.
- Combined rating processing for employees who have changed positions.

## 4. Test Approach and Methodologies

### 4.1. Testing Methodologies

#### **Manual Functional Testing:**
- Execute detailed test cases covering all functional aspects of the workflow.
- Focus on critical user interactions, conditional logic, and exception handling.

#### **Automation Testing:**
- Develop and execute automated tests using Selenium Serenity Cucumber.
- Automate regression tests and end-to-end scenarios after initial manual validation.

#### **Agile Testing Practices:**
- Maintain and manage test cases, steps, and execution records in Rally Agile.
- Use iterative cycles for both manual and automation testing as requirements evolve.

#### **Exploratory Testing:**
- Encourage testers to perform exploratory testing to identify edge cases not covered in the scripted test cases.

### 4.2. Testing Levels
- **Unit Testing:** Performed by developers to verify individual components.
- **Integration Testing:** Validate interactions between application modules.
- **System Testing:** Verify the complete integrated workflow.
- **User Acceptance Testing (UAT):** Confirm system meets requirements.

## 5. Test Items

### **Functional Modules:**
- Performance Rating Plan Cover Sheet workflow.
- Midyear Rating process.
- End‑of‑Year Rating process.

### **Components:**
- Form routing and approval logic.
- Conditional logic based on employee tenure and position changes.
- Email notification system for examiner alerts.
- Bypass functionality for examiner sign-off.

### **Tools & Artifacts:**
- Rally Agile for managing test cases and tracking defects.
- Selenium Serenity Cucumber for automation scripts.
- Test environment and test database for execution.

## 6. Test Deliverables
- **Test Strategy Document**
- **Master Test Plan** (This document)
- **Detailed Test Cases and Steps** (Documented in Rally Agile)
- **Requirements Traceability Matrix (RTM)**
- **Manual Test Execution Records**
- **Automation Test Scripts**
- **Defect/Bug Reports**
- **Test Summary Report**
- **Roles Matrix**

## 7. Test Environment

### **Hardware & Software:**
- Dedicated test environment mirroring production.
- Supported browsers and platforms for UI testing.

### **Data Environment:**
- Dedicated test database containing realistic test data.

### **Other Tools:**
- Rally Agile for test management.
- Selenium Serenity Cucumber for automation.

## 8. Roles and Responsibilities
- **Test Lead:** Planning, coordination, and risk management.
- **Testers:** Execute manual test cases, document results, report defects.
- **Automation Engineers:** Develop and maintain automation scripts.
- **Developers:** Assist in defect resolution and provide technical support.
- **Project Manager:** Ensure resource allocation and oversee testing.
- **Business Analysts/SMEs:** Validate requirements and support UAT.

## 9. Schedule and Milestones
- **Planning Phase:** Finalize Master Test Plan by [Insert Date].
- **Test Case Development:** Complete by [Insert Date].
- **Environment Setup:** Complete by [Insert Date].
- **Manual Testing Execution:** [Insert Date Range].
- **Automation Development:** Start [Insert Date].
- **Regression Testing:** Conducted as new builds are available.
- **UAT and Final Sign-Off:** Complete by [Insert Date].

## 10. Risk Assessment and Mitigation

### **Risks:**
- Delays in test environment setup.
- Incomplete or evolving requirements.
- Integration issues between modules.

### **Mitigation Strategies:**
- Regular status meetings.
- Early test case reviews.
- Backup environments and prioritization.

## 11. Entry and Exit Criteria

### **Entry Criteria:**
- Stable build available.
- Test environment and database setup.
- Test cases and RTM approved.

### **Exit Criteria:**
- All planned test cases executed.
- All critical defects resolved.
- Automated regression tests implemented.
- Successful UAT completion.

## 12. Test Reporting and Communication
- **Daily/Weekly Status Reports**
- **Defect Review Meetings**
- **Test Summary Report**
- **Stakeholder Communication via Rally Agile**

## 13. Approvals
- **Tester:** [Signature/Name]  
- **Project Manager:** [Signature/Name]
