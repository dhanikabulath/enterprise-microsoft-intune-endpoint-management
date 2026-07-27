# Microsoft Intune Endpoint Management Lab

A hands-on Microsoft Intune portfolio demonstrating Windows and macOS endpoint administration in a Microsoft 365 enterprise environment.

This repository documents practical endpoint-management workflows including device enrollment, configuration profiles, compliance policies, application deployment, endpoint security, remote administration, macOS MDM, FileVault encryption, and Windows Autopilot.

---

## Lab Overview

The environment was designed to simulate common responsibilities performed by IT Support, Endpoint Administration, and Microsoft 365 administrators.

The portfolio uses Microsoft Intune and Microsoft Entra ID to centrally manage Windows and macOS endpoints.

### Core Technologies

- Microsoft Intune
- Microsoft Entra ID
- Microsoft 365
- Windows 11
- macOS
- Microsoft Defender Antivirus
- Microsoft Defender Firewall
- BitLocker
- FileVault
- Windows Autopilot
- Microsoft Company Portal
- PowerShell
- VMware Fusion

---

## Lab Architecture

```text
                     Microsoft 365 Tenant
                            │
                            ▼
                    Microsoft Entra ID
                            │
                            ▼
                     Microsoft Intune
                            │
              ┌─────────────┴─────────────┐
              │                           │
              ▼                           ▼
         Windows 11                     macOS
          CLIENT01                   MacBook Air
              │                           │
      ┌───────┼────────┐          ┌───────┼────────┐
      │       │        │          │       │        │
      ▼       ▼        ▼          ▼       ▼        ▼
 Configuration Compliance Security Configuration Compliance FileVault
      │       │        │
      └───────┼────────┘
              │
              ▼
       Windows Autopilot
```

---

# Projects

## Project 01 – Windows Device Enrollment

Enrolled a Windows 11 endpoint into Microsoft Intune and established centralized device management.

### Key Tasks

- Microsoft Entra device registration
- Intune enrollment
- Device inventory verification
- Management-state validation
- Endpoint synchronization
- Device-group configuration

📁 `01-Windows-Device-Enrollment/`

---

## Project 02 – Configuration Profiles & Compliance

Created and deployed Windows configuration and compliance policies.

### Key Tasks

- Windows configuration profiles
- Settings Catalog
- Device restrictions
- Security baseline configuration
- Compliance policy creation
- Group-based policy assignment
- Compliance monitoring
- Policy deployment verification

📁 `02-Configuration-Profiles-and-Compliance/`

---

## Project 03 – Application Deployment

Deployed and managed applications through Microsoft Intune.

### Key Tasks

- Intune application management
- Application assignments
- Required application deployment
- Device-group targeting
- Installation monitoring
- Endpoint-side verification

📁 `03-Application-Deployment/`

---

## Project 04 – Endpoint Security

Implemented centralized endpoint-security controls for the managed Windows 11 endpoint.

### Key Tasks

- Microsoft Defender Antivirus
- Real-time protection
- Behaviour monitoring
- Cloud-delivered protection
- Microsoft Defender Firewall
- Domain, Private, and Public firewall profiles
- BitLocker disk encryption
- TPM-backed encryption
- Security-policy assignment
- Endpoint security monitoring

📁 `04-Endpoint-Security/`

---

## Project 05 – Device Troubleshooting & Remote Administration

Performed practical endpoint troubleshooting and remote administration through Intune.

### Key Tasks

- Device-state investigation
- Policy-status review
- Remote diagnostic collection
- Diagnostic-status monitoring
- Remote restart
- Endpoint troubleshooting workflow

📁 `05-Device-Troubleshooting-and-Remote-Administration/`

---

## Project 06 – macOS MDM, Security & Compliance

Extended the Intune environment to macOS and demonstrated cross-platform endpoint management.

### Key Tasks

- Apple MDM Push Certificate configuration
- Microsoft Company Portal enrollment
- macOS MDM enrollment
- Microsoft Entra device-group configuration
- macOS Settings Catalog
- Passcode and screen-lock policies
- macOS compliance policies
- System Integrity Protection requirements
- FileVault disk encryption
- Recovery-key management
- Policy deployment verification
- Safe MDM unenrollment

📁 `06-macOS-MDM-Security-and-Compliance/`

---

## Project 07 – Windows Autopilot

Configured and tested modern Windows provisioning using Windows Autopilot.

### Key Tasks

- Hardware-hash collection with PowerShell
- Autopilot device registration
- Autopilot device groups
- User-driven deployment profile
- Microsoft Entra Join
- Enrollment Status Page configuration
- Deployment-profile assignment
- Remote Autopilot Reset testing
- Windows OOBE
- Organizational Autopilot recognition
- Sysprep troubleshooting

The remote Autopilot Reset encountered a failure during testing and was retained as troubleshooting evidence rather than represented as a successful deployment. The registered endpoint subsequently reached OOBE and displayed the organizational sign-in experience.

📁 `07-Windows-Autopilot/`

---

# Repository Structure

```text
microsoft-intune-lab/
│
├── 01-Windows-Device-Enrollment/
│   ├── README.md
│   └── Screenshots/
│
├── 02-Configuration-Profiles-and-Compliance/
│   ├── README.md
│   └── Screenshots/
│
├── 03-Application-Deployment/
│   ├── README.md
│   └── Screenshots/
│
├── 04-Endpoint-Security/
│   ├── README.md
│   └── Screenshots/
│
├── 05-Device-Troubleshooting-and-Remote-Administration/
│   ├── README.md
│   └── Screenshots/
│
├── 06-macOS-MDM-Security-and-Compliance/
│   ├── README.md
│   └── Screenshots/
│
├── 07-Windows-Autopilot/
│   ├── README.md
│   └── Screenshots/
│
└── README.md
```

---

# Endpoint Management Lifecycle Demonstrated

```text
Enrollment
    │
    ▼
Identity & Device Registration
    │
    ▼
Configuration
    │
    ▼
Compliance
    │
    ▼
Application Deployment
    │
    ▼
Endpoint Security
    │
    ▼
Monitoring & Troubleshooting
    │
    ▼
Automated Provisioning
```

---

# Technical Skills Demonstrated

### Microsoft Intune

- Device enrollment
- Windows endpoint management
- macOS endpoint management
- Configuration profiles
- Settings Catalog
- Compliance policies
- Application deployment
- Endpoint security policies
- Remote device administration
- Device diagnostics
- Policy monitoring
- Group-based targeting

### Endpoint Security

- Microsoft Defender Antivirus
- Microsoft Defender Firewall
- BitLocker
- FileVault
- TPM-backed encryption
- Security-policy deployment
- Endpoint compliance

### Microsoft Entra ID

- Device identities
- Security groups
- Device-group membership
- Microsoft Entra Join
- Group-based Intune assignments
- Organizational authentication

### Windows Administration

- Windows 11 management
- PowerShell
- Windows Recovery Environment
- Sysprep
- OOBE
- Windows Autopilot
- Endpoint troubleshooting

### Apple Endpoint Management

- Apple MDM Push Certificate
- macOS MDM enrollment
- Company Portal
- macOS security configuration
- FileVault
- macOS compliance management
- MDM unenrollment

---

# Troubleshooting Experience

The labs intentionally include operational troubleshooting rather than only successful configuration screenshots.

Issues investigated during the environment included:

- Delayed Intune device enrollment
- MDM enrollment verification
- Policy deployment delays
- Application installation status
- Device synchronization
- Security-policy targeting
- macOS MDM prerequisites
- Apple MDM Push Certificate configuration
- FileVault recovery-key handling
- Failed remote Autopilot Reset
- Windows Recovery Environment validation
- Sysprep shutdown failure
- Sysprep Panther log analysis
- Windows OOBE recovery
- Autopilot provisioning behaviour

This provides evidence of both administrative configuration and practical troubleshooting.

---

# Portfolio Outcome

This lab demonstrates an end-to-end Microsoft Intune endpoint-management environment covering both Windows and macOS.

The projects progress from basic enrollment and policy management to application deployment, endpoint security, remote troubleshooting, cross-platform MDM, disk encryption, and Windows Autopilot provisioning.

The repository is designed as practical evidence of skills relevant to:

- IT Support
- Service Desk / Help Desk
- Desktop Support
- Junior Systems Administration
- Microsoft 365 Administration
- Endpoint Administration
- Modern Workplace Support

---

## Status

**Completed – 7 Projects**
