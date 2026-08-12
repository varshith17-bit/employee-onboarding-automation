# Employee Onboarding Automation

A Microsoft 365 business application that streamlines employee onboarding using **SharePoint, Power Apps, and Power Automate**.

## Project Overview

The solution provides a centralized employee onboarding system where employee records are stored in SharePoint, surfaced through a Power Apps interface, and used to trigger automated notifications through Power Automate.

## Architecture

```text
Employee record added
        |
        v
SharePoint - Employees List
        |
        +--------------------+
        |                    |
        v                    v
Power Apps              Power Automate
Employee UI             New-item trigger
                            |
                            v
                     Automated email
                     notification
```

## Technologies

- **Microsoft SharePoint** — employee data and onboarding resources
- **Microsoft Power Apps** — employee management application
- **Microsoft Power Automate** — event-driven workflow automation
- **Microsoft 365** — identity, collaboration, and productivity platform

## Implemented Features

- Employee master list
- Employee ID, department, job title, email, joining date, manager, and onboarding status fields
- Power Apps interface connected to the SharePoint Employees list
- Automated workflow triggered when a new employee record is created
- Automated email notification action
- SharePoint navigation for onboarding resources

## SharePoint Structure

The SharePoint site contains onboarding resources such as:

- Onboarding checklist
- Training
- How we work
- Meet the team
- Documents
- Employees

## Automation Flow

**Trigger:** When an item is created in the SharePoint `Employees` list.

**Action:** Send an automated email notification to the configured recipient using the employee information from the newly created item.

## Power Apps

The Power Apps application provides a user interface for viewing and managing employee records stored in SharePoint. The app was generated from the Employees list and includes employee browsing and detail views.

## Security & Privacy

This public repository contains documentation and fictional/sample data only. Real employee personal information, credentials, connection references, and tenant-specific secrets must not be committed to GitHub.

## Deployment

The application is deployed within the Microsoft Power Platform environment. GitHub is used as the public project portfolio and documentation repository; it is not the runtime host for the Power App or Power Automate flow.

## Future Enhancements

- Manager approval workflow
- Automated onboarding task/checklist assignment
- Welcome email with joining information
- Training completion tracking
- Teams notification integration
- Dashboard for onboarding progress

## Author

**Varshith A**

B.Tech — Information Science & Technology (AI & Data Science)