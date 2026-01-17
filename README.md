# flexspace-powerapps
Power Apps solution for managing Work From Home (FlexSpace) requests with multi-level approval, email/Teams notifications, and admin oversight.
# FlexSpace – Work From Home Request Management App

FlexSpace is a Power Apps solution designed to streamline the Work From Home (WFH) request process through a structured approval workflow, automated notifications, and centralized administration.

The application supports request submission, multi-request approval, and administrative monitoring while ensuring data governance and compliance.

---

## Key Features

- Submit Work From Home (FlexSpace) requests
- Manager approval via:
  - Power Apps
  - Outlook email
  - Microsoft Teams
- Bulk approve or reject requests
- Role-based access (Requester, Approver, Admin)
- Centralized request monitoring for administration
- Mobile-friendly via Power Apps mobile app
- Automated data retention and deletion

---

## User Roles & Capabilities

### 1. Requester
- Create new FlexSpace requests
- View request history and request details
- Withdraw submitted requests
- Filter and search requests
- Receive approval status notifications

**Data retention:** 90 days

---

### 2. Approver
- Review pending FlexSpace requests
- Approve or reject requests individually or in bulk
- Filter requests by date, requester, or status
- Take action directly from:
  - Power Apps
  - Outlook email
  - Microsoft Teams activity feed

**Data retention:** 30 days

---

### 3. Admin
- View all submitted requests across the organization
- Monitor approval status and request details
- Support downstream reporting and operational updates
- Manage administrative oversight (read-only)

**Data retention:** 7 days

---

## Approval & Notification Flow

1. Requester submits a FlexSpace request via Power Apps
2. Approver receives notification via:
   - Outlook email
   - Microsoft Teams
3. Approver approves or rejects the request
4. Requester is notified of the final decision
5. Request data is retained based on user role policy

---

## Mobile Access

FlexSpace is fully supported on mobile devices via the Microsoft Power Apps mobile application.

**Steps:**
1. Install Power Apps from App Store or Google Play
2. Connect to corporate VPN (if required)
3. Log in using corporate credentials
4. Search for and open **FlexSpace**

---

## Architecture Overview

- Frontend: Microsoft Power Apps
- Workflow Automation: Power Automate
- Notifications: Outlook & Microsoft Teams
- Authentication: Microsoft Entra ID (Azure AD)
- Data Source: SharePoint / Dataverse (depending on deployment)

---

## Documentation

- User Guide: `docs/FlexSpace_User_Guide.pdf`
- Screenshots: `docs/Screenshots/`
- Governance policies: `governance/`

---

## Data Governance & Retention

- Requester data: Automatically deleted after **90 days**
- Approver data: Automatically deleted after **30 days**
- Admin data: Automatically deleted after **7 days**
- For data export or reporting, contact the Tax Technology team

---

## Deployment Notes

This repository is intended for:
- Internal reference
- Solution documentation
- Architecture and governance review

Power Apps source files and automation flows may be restricted based on organizational policy.

---

## License

Internal use only.  
All rights reserved.
