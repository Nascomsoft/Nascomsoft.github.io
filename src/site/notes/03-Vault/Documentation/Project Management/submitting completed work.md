---
{"dg-publish":true,"permalink":"/03-vault/documentation/project-management/submitting-completed-work/","title":"📄 Submitting Completed Work","tags":["note","completed"],"dg-note-properties":{"aliases":null,"tags":["note","completed"],"dateCreated":"Sat, 31-10-2026, 10:57 PM","keywords":null,"emblem":"📄","title":"📄 Submitting Completed Work"}}
---

<< [[00-Dashboards/documentation dashboard\|documentation dashboard]]

---

>[!info] Quick Links
>- [NASCOMSOFT Task Assignment Dashboard](https://nascomsoft.github.io/01-dashboards/tasks-assignment-dashboard/)
>- [pCloud Web Application](https://my.pcloud.com/)
>- [pCloud Help Center](https://help.pcloud.com/)
>- [GitHub Official Website](https://github.com/)
>- [GitHub Documentation](https://docs.github.com/)

---
## Introduction

At NASCOMSOFT EMBEDDED LTD, employees are required to submit their completed work for review and verification by the Project Manager.

To ensure that project deliverables are properly organized, accessible, and preserved, the company uses two primary platforms:

- **pCloud:** For submitting documents, reports, circuit diagrams, design files, research materials, and other non-code deliverables.
    
- **GitHub:** For storing and managing project source code and related version-controlled files.
    
The platform used for submission depends on the nature of the assigned task.

This guide explains how to submit completed work, organize deliverables, and ensure they are ready for review.

> [!danger] Before You Begin  
> Ensure that you have completed your assigned task and prepared all required deliverables.
> 
> If you need guidance on executing assignments or organizing your working files, read [[03-Vault/Documentation/Project Management/working on assigned tasks\|Working on Assigned Tasks]] first.

---
## 1. Identifying Where to Submit Your Work

Before submitting your work, determine the appropriate destination based on the type of deliverable.

|Type of Deliverable|Submission Platform|
|---|---|
|Research reports and technical documents|pCloud|
|Circuit diagrams and schematics|pCloud|
|Hardware design files and related documentation|pCloud|
|Testing reports and supporting evidence|pCloud|
|Proposals, presentations, and other documents|pCloud|
|Source code and software projects|GitHub|
|Scripts, configuration files, and other version-controlled software resources|GitHub|

Some assignments may require deliverables to be submitted through both platforms.

For example, a firmware development task may require source code to be uploaded to GitHub, while a separately assigned testing report or technical documentation is submitted through pCloud.

> [!IMPORTANT] Submission Requirements  
> Always follow the deliverable requirements specified in your task assignment.
> 
> If you are unsure where a particular file belongs, contact the Project Manager before submitting it.

---
## 2. Submitting Files Through pCloud

Every project has a dedicated **Submissions** folder for receiving completed non-code deliverables.

The link to this folder will be provided in the relevant Project Brief.

Employees must upload their completed work to this location rather than placing files directly into permanent project folders.

### 2.1 Accessing the Submissions Folder

1. Visit the [NASCOMSOFT Task Assignment Dashboard](https://nascomsoft.github.io/01-dashboards/tasks-assignment-dashboard/).
2. Open your weekly task assignment note.
3. Identify the project associated with your completed task.
4. Open the relevant Project Brief.
5. Locate the **Submissions Folder** link.
6. Follow the link to the designated pCloud submission location.

Depending on the access method configured by the Project Manager, you may be required to sign in to your pCloud account before uploading files.

### 2.2 Uploading Your Deliverables

Once you have accessed the designated submissions location:

1. Select the option to upload files.
2. Choose the completed files from your computer.
3. Wait for the upload process to finish.
4. Confirm that the correct files have been uploaded successfully.
5. Notify the Project Manager that your work is ready for review.

Submit all files required to evaluate your completed task.

If your deliverables contain several related files, organize them in a clearly named folder or compressed archive where appropriate.

### 2.3 File Naming Conventions

Use descriptive filenames that make it easy to identify the project, task, employee, and version of the submitted work.

**Recommended format:**

`ProjectName_TaskDescription_EmployeeName_Version`

**Examples:**

- `GrassCutter_CircuitDesign_John_v1.pdf`
- `IoTSystem_TestReport_Mary_v1.docx`
- `SolarProject_ResearchReport_David_v2.pdf`
- `RobotArm_MechanicalDesign_John_v1.zip`

Avoid generic filenames such as `final.docx`, `newfile.pdf`, or `project1.zip`.

Where revisions are necessary, use clear version numbers to distinguish updated submissions from previous versions.

### 2.4 Submission Rules

All employees are expected to follow these rules:

- Submit work only to the designated project submissions location.
- Ensure that all required files are included.
- Use clear and descriptive filenames.
- Do not modify, overwrite, or delete another employee's submissions.
- Do not move submitted files into permanent project folders without authorization.
- Submit revised files when corrections are requested.
- Notify the Project Manager after completing a submission.

> [!IMPORTANT] Submission Is Not Approval  
> Uploading your work to pCloud does not automatically mean your task has been marked as completed.
> 
> The Project Manager must review and verify the submitted deliverables before confirming task completion.

---

## 3. Submitting Source Code Through GitHub

NASCOMSOFT uses GitHub to store and manage source code developed for company projects.

Employees assigned programming or other code-related tasks must ensure that their work is available in the appropriate repository under the company's GitHub organization.

Source code should not be stored solely on an employee's personal computer or personal GitHub repository.

### 3.1 GitHub Account and Repository Access

Before submitting code, you must:

1. Have a personal [GitHub account](https://github.com/signup).
2. Contact the designated GitHub Administrator to request the necessary access.
3. Confirm that you have permission to access or create the appropriate company project repository.
4. Follow any repository management instructions provided by the GitHub Administrator.

> [!info] Repository Access  
> Access to company repositories is managed by the designated GitHub Administrator.
> 
> Employees must not create company project repositories under their personal accounts as a substitute for the approved company repository.

For additional guidance, see [[Getting Started with GitHub\|Getting Started with GitHub]].

### 3.2 Uploading Source Code

Once you have access to the appropriate repository:

1. Open or clone the assigned company project repository.
2. Add or update the files relevant to your assigned task.
3. Ensure that the necessary source files, configuration files, and dependencies are properly organized.
4. Review your changes and perform relevant tests where applicable.
5. Commit and push your changes to the appropriate branch, following the repository's established workflow.
6. Create a pull request if required by the project workflow.
7. Provide the repository link, branch, commit, or pull request reference to the Project Manager for review.

> [!IMPORTANT] Code Submission  
> Ensure that your latest work has been pushed to the company repository.
> 
> Code that exists only on your local computer or in an unapproved personal repository is not considered properly submitted.

### 3.3 Source Code Submission Guidelines

Before submitting code:
- Confirm that the code is relevant to the assigned project.
- Ensure that the necessary source files are included.
- Use meaningful commit messages.
- Avoid uploading unnecessary temporary files or generated build outputs unless required.
- Do not commit passwords, API keys, access tokens, or other sensitive credentials.
- Include any necessary instructions for building, running, or testing the software when required by the assignment.
- Follow repository instructions provided by the GitHub Administrator.

Where a task involves multiple contributors, coordinate changes to avoid conflicting or duplicated work.

---
## 4. Notifying the Project Manager

After submitting your deliverables, notify the Project Manager that the work is ready for review.

Your notification should clearly identify:

1. The project name.
2. The completed task.
3. Where the deliverables have been submitted.
4. Any relevant information needed for verification.

For GitHub submissions, include the relevant repository and commit or pull request reference where applicable.

For pCloud submissions, identify the submitted files or folder.

**Example:**

> Project: Autonomous Grass Cutter
> 
> Task: Motor Control Firmware Development
> 
> Status: Submitted for Review
> 
> Deliverables: Source code pushed to the company GitHub repository.
> 
> Reference: [Repository or Pull Request Link]

Employees should not wait until the weekly Monday meeting to notify the Project Manager of completed work.

---
## 5. Corrections and Resubmissions

After reviewing your work, the Project Manager may request corrections, additional files, or further testing.

If corrections are required:

1. Review the feedback provided.
2. Make the necessary changes.
3. Verify that the identified issues have been addressed.
4. Resubmit the updated deliverables through the appropriate platform.
5. Notify the Project Manager that the revised work is ready for another review.

For pCloud submissions, use a new version number or another clearly identifiable filename.

For GitHub submissions, push the required changes to the appropriate branch and update the relevant pull request or review reference.

> [!info] Revised Work  
> A task requiring corrections remains subject to verification until the Project Manager accepts the deliverables.

---
## 6. Frequently Asked Questions

**Where should I upload my completed work?**

Use the dedicated pCloud submissions folder for non-code deliverables and the appropriate company GitHub repository for source code.

**Where can I find the pCloud submissions folder?**

The link will be provided in the relevant Project Brief.

**What if I do not have access to the company GitHub repository?**

Contact the designated GitHub Administrator to request access.

**Can I submit source code through pCloud instead of GitHub?**

The standard company workflow requires source code to be maintained in the appropriate company GitHub repository. Contact the Project Manager if an exception is necessary.

**What if my task involves both source code and documentation?**

Submit each required deliverable to its appropriate platform, as specified in your task assignment.

**What if I accidentally upload the wrong file?**

Notify the Project Manager and provide the correct file. Do not overwrite or delete files unless authorized.

**Does submitting my work mean my task is completed?**

No. The Project Manager must review and accept the submitted work before updating its completion status.

**What happens if my work is rejected or requires corrections?**

Review the feedback, make the required changes, and resubmit the work for verification.

---
## What's Next?

After submitting your deliverables, the Project Manager will review the work and determine whether it meets the requirements of the assigned task.

**Continue Reading:** [[03-Vault/Documentation/Project Management/review and verification\|review and verification]]

---

**Remember:** Completing your work is only part of the process. Ensure that your deliverables are submitted to the correct platform, properly organized, and made available for review.