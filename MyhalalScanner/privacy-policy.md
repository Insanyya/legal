tittle : PRIVACY POLICY — MyHalalScanner


Last updated: April 20, 2026

Developer:insanyya.support@gmail.com

This Privacy Policy applies to both versions of the app:
  • MyHalalScanner (Free) — available on Google Play
  • MyHalalScanner Premium (Pro) — available on Google Play

By using this app you agree to the practices described in this policy.
If you do not agree, please uninstall the app and discontinue use.

--------------------------------------------------------------------------------
1. OVERVIEW
--------------------------------------------------------------------------------

MyHalalScanner is an Android application that helps Muslim consumers determine
whether a food product is halal by scanning barcodes or photographing ingredient
labels. The app works primarily on your device using local data files and only
contacts the internet to fetch product information from the OpenFoodFacts open
food database.

We are committed to protecting your privacy. This policy explains exactly what
data is collected, how it is used, and your rights over it.

--------------------------------------------------------------------------------
2. DATA WE COLLECT AND HOW IT IS USED
--------------------------------------------------------------------------------

2.1  DATA STORED LOCALLY ON YOUR DEVICE
----------------------------------------

When you scan a product, the following information is saved to a local database
on your device (SQLite):

  • Product barcode (EAN/UPC)
  • Product name and brand
  • Ingredient list text
  • Scan verdict (Halal / Haram / Doubtful / Unknown)
  • Detected concern keywords (e.g. "gelatin", "E120")
  • Scan date and time
  • Product image URL (a link to the OpenFoodFacts image, not a local copy)
  • Product category and country of sale

This data is stored ONLY on your device. It is never transmitted to our servers.
It is used solely to display your scan history inside the app so you can look up
products you have scanned before without an internet connection.

You can delete individual entries or clear your entire history at any time from
the History screen.

2.2  DATA SENT OVER THE INTERNET
----------------------------------

When you scan a barcode or search for a product, the app contacts the
OpenFoodFacts API (world.openfoodfacts.org) to fetch product information.
The request includes:

  • The product barcode
  • Your preferred language code (e.g. "fr", "en", "ar") so the server can
    return ingredient text in your language
  • A User-Agent string identifying the app ("OpenFoodFactsEditor halal scanner
    app / halalappschak@gmail.com") as required by the OpenFoodFacts API terms

No personal information (name, email, device ID, location) is included in
these requests. OpenFoodFacts is an independent open-source nonprofit project.
Their privacy policy is available at: https://world.openfoodfacts.org/privacy

2.3  CAMERA AND PHOTOS
------------------------

The app requests camera permission to:
  (a) Scan product barcodes using the device camera
  (b) Photograph ingredient labels for OCR text recognition (Premium and Free)
  (c) Capture product photos when contributing to OpenFoodFacts (optional)

  • For barcode scanning and OCR: the camera image is processed entirely on
    your device. The pixel data is NEVER sent to any server. ML Kit (Google's
    on-device machine learning library) processes the image locally.

  • For OCR ingredient scans: a temporary photo may be saved to your device's
    internal app storage (not accessible to other apps or the gallery) while
    the scan is in progress. This photo is only uploaded to OpenFoodFacts if
    you explicitly choose to contribute the product using the "Add to database"
    feature, and only after your confirmation.

  • The app does not access, read, or use any photos already stored in your
    device's gallery or photo library.

2.4  PRODUCT CONTRIBUTIONS TO OPENFOODFACTS (OPTIONAL)
--------------------------------------------------------

If you choose to add or edit a product on OpenFoodFacts (via the built-in
product editor), the following data is sent to OpenFoodFacts:

  • The product barcode
  • The ingredient text you entered or OCR-captured
  • Any photos you choose to upload (product front, ingredient label, nutrition)
  • A shared contributor account identifier (this is not tied to your personal
    identity — all app contributions appear under the same shared account)

This data is submitted to OpenFoodFacts under their open database license
(Open Database License / ODbL). Once submitted, it becomes part of the public
OpenFoodFacts database and is subject to OpenFoodFacts' own privacy and data
policies.

This feature is entirely optional. You can use the halal scanning features
without ever contributing to OpenFoodFacts.

2.5  SETTINGS AND PREFERENCES
--------------------------------

The app stores the following settings in your device's local SharedPreferences
storage (never transmitted off-device):

  • Your selected UI language
  • Dark mode preference
  • Per-category scan toggles (pork, meat, insects, alcohol, vinegar, rennet)
  • GDPR consent status (Free version only)

2.6  ADVERTISING (FREE VERSION ONLY)
--------------------------------------

The free version of MyHalalScanner displays advertisements served by Google
AdMob. To serve these ads, Google AdMob may collect and process:

  • Advertising ID (GAID) — a resettable device identifier
  • IP address (used to estimate approximate location for ad targeting)
  • Information about the ads shown to you and your interaction with them
  • Device information (OS version, screen size, language)

This data is collected and processed by Google, not by us. Google's data
collection is governed by Google's Privacy Policy:
https://policies.google.com/privacy

You can opt out of personalised advertising at any time by:
  • Opening Android Settings → Privacy → Ads → Opt out of Ads Personalisation
  • Or by resetting your Advertising ID in the same menu

In regions subject to GDPR (European Economic Area and UK), the free version
shows a consent dialog before loading any ads. You can withdraw or change your
consent at any time from Settings → Privacy / Consent inside the app.

The Premium version of the app contains NO advertising and Google AdMob is NOT
initialised. No advertising-related data is collected in the Premium version.

--------------------------------------------------------------------------------
3. DATA WE DO NOT COLLECT
--------------------------------------------------------------------------------

We explicitly do NOT collect or have access to:

  • Your name, email address, or any account information
  • Your precise or approximate GPS location
  • Your contacts, calendar, or messages
  • Your browsing history or data from other apps
  • Health or biometric data
  • Payment information (app purchases go through Google Play — we never see
    payment details)
  • Any data from your photo gallery or file system beyond camera captures
    initiated by you within the app

The app does NOT require you to create an account or log in.

--------------------------------------------------------------------------------
4. THIRD-PARTY SERVICES AND THEIR PRIVACY POLICIES
--------------------------------------------------------------------------------

The following third-party services are used by the app. Each has its own
privacy policy that governs how they handle data:

  Service                    | Used in        | Purpose
  ---------------------------|----------------|-----------------------------------
  OpenFoodFacts API          | Free + Premium | Product data (ingredients, images)
  Google AdMob               | Free only      | Advertising
  Google UMP (Consent SDK)   | Free only      | GDPR consent management
  Google ML Kit (on-device)  | Free + Premium | Barcode scanning, OCR, language ID
  Google Play Services       | Free + Premium | App delivery and updates

  OpenFoodFacts privacy policy:
    https://world.openfoodfacts.org/privacy

  Google privacy policy (covers AdMob, UMP, ML Kit, Play Services):
    https://policies.google.com/privacy

  Google AdMob partner policies:
    https://support.google.com/admob/answer/6128543

ML Kit runs ENTIRELY ON YOUR DEVICE. The barcode scanning, text recognition
(OCR), and language detection models do not send any image or text data to
Google servers. ML Kit processes data locally only.

--------------------------------------------------------------------------------
5. DATA RETENTION AND DELETION
--------------------------------------------------------------------------------

5.1  Local scan history
  Your scan history is stored on your device indefinitely until you delete it.
  You can delete individual scan entries by swiping left on any item in the
  History screen, or clear all history via History → Menu → Clear All.
  The app automatically limits history to 500 entries to prevent unbounded
  growth; the oldest entries are removed first when the limit is reached.

5.2  App data and preferences
  All app preferences and settings are deleted when you uninstall the app.

5.3  OpenFoodFacts contributions
  If you submitted product data to OpenFoodFacts, that data is stored by
  OpenFoodFacts under their open database policies. To request deletion of
  contributed data, contact OpenFoodFacts directly at contact@openfoodfacts.org.

5.4  AdMob data (Free version)
  Advertising data held by Google is subject to Google's retention policies.
  Visit https://myaccount.google.com to manage Google's data about you.

--------------------------------------------------------------------------------
6. YOUR RIGHTS (GDPR AND OTHER REGULATIONS)
--------------------------------------------------------------------------------

If you are located in the European Economic Area (EEA), the United Kingdom,
or other jurisdictions with privacy rights legislation, you have the right to:

  • Access: request a copy of data we hold about you
  • Rectification: correct inaccurate data
  • Erasure ("right to be forgotten"): request deletion of your data
  • Restriction: request that we limit how we use your data
  • Portability: receive your data in a machine-readable format
  • Objection: object to our processing of your data
  • Withdraw consent: at any time, for consent-based processing (e.g. ad
    personalisation in the Free version)

Since all personal data is stored locally on your device, you can exercise
most of these rights directly within the app (deleting history, clearing
preferences) without needing to contact us.

For any requests related to data processed by third parties (Google AdMob,
OpenFoodFacts), please contact those services directly using the links in
Section 4.

For any privacy requests or concerns, contact us at: insanyya.support@gmail.com
We will respond within 30 days.

For the Free version's advertising consent, you can:
  • Change or withdraw consent: Settings → Privacy / Consent (inside the app)
  • Reset your Advertising ID: Android Settings → Privacy → Ads

--------------------------------------------------------------------------------
7. CHILDREN'S PRIVACY
--------------------------------------------------------------------------------

MyHalalScanner is not directed at children under the age of 13 (or 16 in the
EEA). We do not knowingly collect personal information from children.

If you are a parent or guardian and believe your child has provided personal
information through this app, please contact us at insanyya.support@gmail.com and
we will take appropriate steps to delete such information.

The Free version's advertising is configured with Google AdMob's standard
audience settings and does not serve personalised ads to users who have not
consented.

--------------------------------------------------------------------------------
8. DATA SECURITY
--------------------------------------------------------------------------------

All data stored on your device (scan history, preferences) is stored in the
app's private internal storage. It is not accessible to other apps or readable
without root access to the device.

Data sent to OpenFoodFacts and Google AdMob is transmitted over HTTPS (TLS).
The app's network security configuration explicitly disables cleartext (HTTP)
traffic.

We do not operate any servers that store your personal data, so there is no
server-side security risk from our side. The security of your data on your
device depends on your device's own security (screen lock, encryption, etc.).

--------------------------------------------------------------------------------
9. INTERNATIONAL DATA TRANSFERS
--------------------------------------------------------------------------------

When the app contacts OpenFoodFacts servers or Google's advertising
infrastructure, your request data may be processed on servers located outside
your country, including in the United States and the European Union.

OpenFoodFacts is a French nonprofit and its primary servers are based in the EU.
Google operates data centres globally. Both have data transfer mechanisms in
place that comply with applicable data protection law (Standard Contractual
Clauses, adequacy decisions, etc.).

--------------------------------------------------------------------------------
10. CHANGES TO THIS PRIVACY POLICY
--------------------------------------------------------------------------------

We may update this Privacy Policy from time to time to reflect changes in
the app's features or applicable law. When we make significant changes:

  • The "Last updated" date at the top of this document will be revised
  • If the change materially affects how we handle personal data, we will
    provide notice within the app or via the Play Store listing

We encourage you to review this policy periodically.

Continued use of the app after a policy update constitutes your acceptance of
the revised policy.

--------------------------------------------------------------------------------
11. CONTACT
--------------------------------------------------------------------------------

For any questions, concerns, or requests regarding this Privacy Policy or
the handling of your data, please contact:

  Developer:  insanyya.support@gmail.com

We aim to respond to all privacy-related inquiries within 30 days.

END OF PRIVACY POLICY

