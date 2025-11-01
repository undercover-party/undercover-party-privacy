# Google Play Store - Data Safety Declaration
## UnderCover Party

This document helps you fill out the Data Safety section in Google Play Console.

---

## Question 1: Does your app collect or share any of the required user data types?

**Answer: YES** ✅

---

## Question 2: Is all of the user data collected by your app encrypted in transit?

**Answer: YES** ✅

All data is transmitted via HTTPS/TLS encryption:
- Firebase Authentication: OAuth 2.0 over HTTPS
- RevenueCat: HTTPS
- Google AdMob: HTTPS

---

## Question 3: Do you provide a way for users to request that their data is deleted?

**Answer: YES** ✅

**URL:** `https://arouaystudio.github.io/undercover-party-privacy/delete-account.html`
(or wherever you host your delete-account.html page)

**Email:** arouaystudio@gmail.com

---

## Question 4: Do you provide a way for users to request deletion of some or all of their data without having to delete their account? (Optional)

**Answer: YES** ✅

**Explanation:** Users can request deletion of:
- **Purchase data** (via email to arouaystudio@gmail.com) - Account remains active, but premium access is lost
- **Advertising data** (via Google My Ad Center) - Account remains active

**Note:** Authentication data (email, name, profile picture) cannot be deleted without deleting the account, as these are essential for account functionality.

---

## Data Types Collected

### 1. **Personal Info**

#### Email addresses
- **Collected:** YES ✅
- **Shared with third parties:** YES (RevenueCat, Apple/Google payment processors)
- **Purposes:**
  - ✅ App functionality
  - ✅ Account management
- **Optional or Required:** REQUIRED (for accounts and subscriptions)
- **Can users request deletion:** YES ✅

#### Name
- **Collected:** YES ✅
- **Shared with third parties:** NO
- **Purposes:**
  - ✅ App functionality
  - ✅ Personalization
- **Optional or Required:** OPTIONAL (from Google profile)
- **Can users request deletion:** YES ✅

---

### 2. **Photos and videos**

#### Profile picture
- **Collected:** YES ✅
- **Shared with third parties:** NO
- **Purposes:**
  - ✅ App functionality
  - ✅ Personalization
- **Optional or Required:** OPTIONAL (from Google profile)
- **Can users request deletion:** YES ✅

---

### 3. **Financial info**

#### Purchase history
- **Collected:** YES ✅
- **Shared with third parties:** YES (RevenueCat)
- **Purposes:**
  - ✅ App functionality
  - ✅ Account management
- **Optional or Required:** OPTIONAL (only if user purchases premium)
- **Can users request deletion:** YES (subject to 12-month legal retention) ✅

---

### 4. **App activity**

#### In-app search history
- **Collected:** NO ❌

#### Installed apps
- **Collected:** NO ❌

#### Other user-generated content
- **Collected:** NO ❌

#### Other actions
- **Collected:** YES ✅ (Ad interactions)
- **Shared with third parties:** YES (Google AdMob)
- **Purposes:**
  - ✅ Advertising or marketing
- **Optional or Required:** REQUIRED (for ad-supported experience)
- **Can users request deletion:** YES (via Google My Ad Center) ✅

---

### 5. **Device or other identifiers**

#### Device or other IDs
- **Collected:** YES ✅
- **Shared with third parties:** YES (Google AdMob, RevenueCat, Firebase)
- **Purposes:**
  - ✅ App functionality
  - ✅ Analytics
  - ✅ Advertising or marketing
  - ✅ Account management
- **Optional or Required:** REQUIRED
- **Can users request deletion:** YES ✅

**Types of IDs collected:**
- Firebase User ID (authentication)
- Google User ID (from Google Sign-In)
- Advertising ID (for AdMob)
- Device ID (for subscription verification)

---

## Account Creation Methods

**Question:** Parmi les méthodes de création de compte suivantes, lesquelles votre appli prend-elle en charge ?

**Answer:** ✅ **OAuth**

**Explanation:** You use Google Sign-In (OAuth 2.0) via Firebase Authentication.

---

## Account Deletion URL

**Question:** Ajoutez un lien permettant aux utilisateurs de demander la suppression de leur compte

**URL:**
```
https://arouaystudio.github.io/undercover-party-privacy/delete-account.html
```

(Replace with your actual hosted URL)

**Alternative:** If you don't have a website yet, you can use:
```
mailto:arouaystudio@gmail.com?subject=Account%20Deletion%20Request
```

---

## Privacy Policy URL

**URL:**
```
https://arouaystudio.github.io/undercover-party-privacy/index.html
```

(Replace with your actual hosted URL)

---

## Third-Party SDKs to Declare

### 1. Google Firebase Authentication
- **Purpose:** User authentication
- **Data shared:** Email, name, profile picture, Google User ID

### 2. RevenueCat
- **Purpose:** Purchase management (one-time premium purchase)
- **Data shared:** Email, Firebase User ID, purchase history

### 3. Google AdMob
- **Purpose:** Advertising
- **Data shared:** Advertising ID, device info, IP address, ad interactions

---

## Important Notes

1. **Be Consistent:** Make sure your Play Store declarations match your privacy policy exactly

2. **Test the URLs:** Before submitting, verify that your privacy policy and account deletion pages are accessible online

3. **Update Regularly:** If you add new features or data collection, update both your privacy policy and Play Store declaration

4. **Apple App Store:** You'll need to make similar declarations in App Store Connect (see separate section below)

---

## Apple App Store - App Privacy Declaration

For App Store Connect, declare the following in the **App Privacy** section:

### Contact Info
- **Email Address**
  - ✅ Used for app functionality
  - ✅ Used for account management
  - ✅ Linked to user identity
  - ✅ Shared with RevenueCat, Apple/Google payment processors

- **Name**
  - ✅ Used for app functionality
  - ✅ Used for personalization
  - ✅ Linked to user identity
  - ❌ Not shared with third parties

### User Content
- **Photos or Videos** (profile picture only)
  - ✅ Used for app functionality
  - ✅ Used for personalization
  - ✅ Linked to user identity
  - ❌ Not shared with third parties

### Purchases
- **Purchase History**
  - ✅ Used for app functionality
  - ✅ Linked to user identity
  - ✅ Shared with RevenueCat

### Identifiers
- **User ID** (Firebase User ID, Google User ID)
  - ✅ Used for app functionality
  - ✅ Used for analytics
  - ✅ Linked to user identity
  - ✅ Shared with Firebase, RevenueCat

### Usage Data
- **Advertising Data**
  - ✅ Used for advertising
  - ✅ Linked to user identity
  - ✅ Shared with Google AdMob

---

## Compliance Checklist

Before submitting to stores:

- [ ] Privacy policy updated with Firebase Authentication ✅
- [ ] Privacy policy updated with RevenueCat ✅
- [ ] Account deletion page created ✅
- [ ] Privacy policy and deletion page hosted online
- [ ] Play Store Data Safety filled out
- [ ] App Store App Privacy filled out
- [ ] Both declarations match privacy policy
- [ ] Account deletion flow tested
- [ ] Privacy policy link added to app (usually in Settings)
- [ ] Consent dialog for GDPR (EU users under 16) implemented

---

## Contact for Questions

**Email:** arouaystudio@gmail.com
**Developer:** Maher AROUAY

---

*Last Updated: November 1, 2025*
