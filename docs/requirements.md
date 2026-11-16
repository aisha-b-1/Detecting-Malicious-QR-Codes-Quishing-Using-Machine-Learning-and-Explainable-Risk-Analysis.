QRGuard – Requirements

Method: MoSCoW · R1 = December · R2 = January–February · R3 = if time allows

Must have (R1)

Decoding

FR-01 Upload a QR image (PNG/JPEG, incl. phone photo)
FR-02 Decode the QR code without opening the link
FR-03 Show the full link
FR-04 Highlight the real domain
FR-05 Message if no QR code is found
FR-06 Message if the content is not a web link

Security checks

FR-07 Flag links without HTTPS
FR-08 Flag IP addresses instead of domain names
FR-09 Flag URL shorteners
FR-10 Flag lookalike brand domains
FR-11 Flag punycode (xn--) domains
FR-12 Flag suspicious structure (@, many subdomains, very long URL)

Verdict

FR-13 Give a verdict: Safe / Suspicious / Dangerous
FR-14 Explain every warning in plain English
FR-15 Give advice for each verdict
FR-16 Proceed link only for Safe or Suspicious
FR-17 Confirm warning before proceeding on Suspicious

Non-functional

NFR-01 Accept only PNG/JPEG up to 5 MB
NFR-02 Check the file is a real image
NFR-03 Do not store images or links
NFR-04 Never visit the scanned link
NFR-05 Display QR content safely (no code injection)
NFR-06 No debug mode or error details shown to users
NFR-07 App keeps working after bad input
NFR-08 Use colour + text + icon for verdicts
NFR-09 Use plain, jargon-free language
NFR-10 Each check is a separate, tested function
Should have (R2)

Extra checks

FR-18 Check Google Safe Browsing
FR-19 Never show "Safe" if a check fails
FR-20 Flag newly registered domains
FR-21 Follow shortened links safely
FR-22 Machine learning prediction

Organisation verification

FR-23 Read the organisation name from the sign (OCR)
FR-24 Match the name to the registry
FR-25 Verified if domains match, Dangerous if not
FR-26 Show the official website on a mismatch
FR-27 Admin can manage the registry

Non-functional

NFR-11 Works on phone, tablet and desktop
NFR-12 Result within 3 seconds
NFR-13 Same link always gives the same result
NFR-14 4 of 5 test users understand the result (ethics approval needed)
NFR-15 HTTPS when deployed
NFR-16 Hashed admin passwords
NFR-17 Rate limiting
NFR-18 API keys kept out of code
NFR-19 ML: ≥ 90% detection, < 5% false positives
Could have (R3)
FR-28 Live camera scanning
FR-29 Manual URL entry
FR-30 Show what influenced the ML prediction
FR-31 Multilingual support
FR-32 QR codes in emails or PDFs
Won't have
FR-33 User accounts or scan history (privacy)
FR-34 Native mobile app
FR-35 Visiting or analysing destination pages (safety)