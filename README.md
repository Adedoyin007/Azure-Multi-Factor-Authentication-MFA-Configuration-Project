# Azure-Multi-Factor-Authentication-MFA-Configuration-Project
Azure Multi-Factor Authentication (MFA)  Configuration Project
# Azure Multi-Factor Authentication (MFA) Configuration Project

## Overview
This project demonstrates the implementation of Multi-Factor Authentication (MFA) in Microsoft Azure (Microsoft Entra ID). MFA enhances security by requiring users to verify their identity using multiple authentication methods.

---

## Objectives
- Configure Multi-Factor Authentication in Azure
- Enable multiple authentication methods
- Test and validate MFA during login
- Understand limitations of Azure free tier

---

## Configuration Steps

1. Logged into Azure Portal
2. Navigated to Microsoft Entra ID
3. Selected Users → Authentication Methods
4. Enabled Microsoft Authenticator
5. Set Microsoft Authenticator as default sign-in method
6. Added backup authentication method (Email)

---

## Authentication Methods Configured

- Microsoft Authenticator (Primary)
- Email (Backup)

---

## Testing MFA

The MFA configuration was tested by logging out and signing back in.

### Test Process:
1. Entered username and password
2. MFA prompt appeared requesting approval
3. Number matching challenge was displayed
4. Approved request using Microsoft Authenticator app
5. Successfully logged into Azure portal

---

## Conditional Access Limitation

Conditional Access policies could not be configured because the Azure account is using the free tier. This feature requires Microsoft Entra ID Premium licensing.

---

## Security Justification

- Microsoft Authenticator is more secure than SMS or email because it reduces the risk of phishing and SIM swap attacks.
- Number matching adds an extra layer of protection against unauthorized approvals.

---

## Troubleshooting

**Issue:** Unable to create Conditional Access policies  
**Cause:** Free tier does not include required licensing  
**Resolution:** Proceeded with MFA-only configuration and documented the limitation  

---

## Conclusion

MFA was successfully implemented and tested. The system now requires a second verification step during login, significantly improving account security.
