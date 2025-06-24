# 📧 Phishing Email Analysis Report

**Date:** June 24, 2025  
**Time:** 10:15 PM  
**Analyst:** Jeyashree.M  
**Sample Type:** Text-based phishing email (realistic format)

---

## 🧪 Step-by-Step Analysis

### 1. Sender Check (Spoofing)
- **From:** `appleid@apple.com`
- **Return-Path:** `notice@account-verify-apple.com`
- **Analysis:**  
  - Looks like Apple, but the **Return-Path domain is different** from the From address.
  - Shows signs of **email spoofing**.
  - ❌ **Suspicious sender** identity.

---

### 2. Header Check (SPF, DKIM, DMARC)
- **SPF:** FAIL  
- **DKIM:** NONE  
- **DMARC:** FAIL  
- **Server IP:** `185.61.123.7` (from suspicioushost.ru)  
- **Analysis:**  
  - Email failed **all 3 security checks**, meaning the sender is not verified.
  - IP address is not from Apple’s trusted infrastructure.
  - ❌ Indicates this email is highly likely to be spoofed.

---

### 3. Suspicious Links or Attachments
- **Link in email:**  
  - Displayed: `https://appleid-security-login.com/verify`
- **Analysis:**  
  - Domain **looks like Apple** but is **not `apple.com`**.
  - A classic **phishing link** designed to steal login details.
  - ❌ Dangerous phishing site.

---

### 4. Urgent or Threatening Language
- “Your Apple ID has been locked”  
- “Verify immediately”  
- “Account will be permanently suspended”  
- **Analysis:**  
  - Classic scare tactics used to **force the user to act quickly**.
  - ❌ Typical phishing pressure.

---

### 5. Mismatched URLs
- Link Text: `Click the link to unlock your account`
- Actual Link: `https://appleid-security-login.com/verify`
- **Analysis:**  
  - **Domain looks legitimate** but is **actually fake**.
  - **Does not match official Apple domains**.
  - ❌ URL mismatch — designed to trick the user.

---

### 6. Grammar & Personalization
- Greeting: “Dear Jeyashree” ✅ (personalized)  
- Language: Slightly robotic, formal  
- **Analysis:**  
  - Better grammar than typical phishing, but still lacks **Apple's professional tone**.
  - ⚠️ Slightly suspicious.

---

### 7. Attachments
- **No attachments found.**  
- ✅ Safe from file-based malware in this case.

---

## ✅ 8. Final Summary of Phishing Traits
| 🔍 Trait                    | ✅ Found? | 📝 Description                                              |
|----------------------------|-----------|---------------------------------------------------------------|
| Spoofed Sender             | ✅ Yes    | Return-Path does not match the From address                   |
| SPF/DKIM/DMARC Failed      | ✅ Yes    | Email failed all 3 authentication checks                      |
| Suspicious Link            | ✅ Yes    | URL looks like Apple, but it's not a real Apple domain        |
| Urgent Language            | ✅ Yes    | Threatens account lock and permanent suspension               |
| Mismatched URL             | ✅ Yes    | Link text vs actual link domain do not match                  |
| Grammar & Personalization | ⚠️ Partial | Slightly robotic language, though name is used                |
| Attachments Present        | ❌ No     | No attachments found in the email                             |

---

## 🛑 Conclusion

This email is a **high-risk phishing attempt** designed to steal the recipient’s Apple ID login.  
Signs of spoofing, failed security authentication, and fake URLs confirm it is **not legitimate**.

> 🚫 **Do not click links or reply to this email.**

