# Elevate-Labs-Task-6

DATE : 12.08.2025

Objective -  Understand what makes a password strong and test it against password strength tools.

Tool used : https://passwordmeter.com

STEP 1- Create multiple passwords with varying complexity.
Complexity Types:
-->Very weak (bad): password, 123456 — easy baseline.

-->Weak: jeny2022, passw0rd — small variations on words/numbers.

-->Medium: BlueCar7! or tR0ub4dor — some mixing of case/numbers/symbols.

-->Strong (random): G7$kL9!rQ2 — random chars, length ~10+.

-->Passphrase: correct horse battery staple (example of style — don’t reuse this exact phrase).

this range shows how length, unpredictability and character variety change measured “strength.” Use these to compare checkers and learn what they flag.

STEP 2-Use uppercase, lowercase, numbers, symbols, and length variations.

Character classes: lowercase (26), uppercase (26), digits (10), symbols (~32–33 common). 
More classes → larger character set → higher theoretical entropy.

Length matters more than adding a single symbol. Example patterns to try:

aaaaaa (6 chars, one class)

Abc123 (6 chars, 3 classes)

Abc123!@ (8 chars, 4 classes)

word-word-word-word (passphrase style, 4 words, often long and memorable)

STEP 3- Test each password on password strength checker.

Tool used(Passwordmeter.com ) -- PasswordMeter uses a rule-based scoring system. It computes a score out of 100 using a series of additive bonuses and penalties, based on specific characteristics of the password

STEP 4 - Note scores and feedback from the tool.

RULES For (passwordmeter.com)
Additions (Bonuses):
Length: Adds +4 points per character — longer passwords score more.

Uppercase Letters: If not all characters are uppercase, adds ((len − uppercase_count) * 2) — rewarding mixed cases.

Lowercase Letters: Adds ((len − lowercase_count) * 2) — similar logic for lowercase.

Numbers: Adds +4 points per digit, if mixed with letters.
 
Symbols: Adds +6 points per symbol — symbols are weighted heavily.

Middle Numbers or Symbols: Adds +2 points per occurrence — encouraging placing them in the center.

Requirements Met: Additional +2 points per requirement met (length ≥8, plus meeting at least 3 of the 4 categories: uppercase, lowercase, numbers, symbols).

Deductions (Penalties):
Applies negative points for:

Letters only or Numbers only: simple deductions (−n points).

Repeated characters, consecutive uppercase/lowercase/numbers: each costs −2 points per run.

Sequential letters/numbers/symbols (three or more in a row): each sequence subtracts −3 points 
Password Meter +1

STEP 5- Identify best practices for creating strong passwords
 I created a password : Xi6$eZ0@oK3 with satisfies the Rules of Additions (Bonus) and Deductions (Penalities)

 STEP 6- Write down tips learned from the evaluation.

-->Length buys more security than a single symbol.

-->Randomness beats clever substitutions.

-->Passphrases (4 random words) are memorable and strong.

-->If a checker flags “found in breach,” change it immediately and stop reusing it.

-->Use a password manager + MFA = very high practical security for most users.

STEP 7- Research common password attacks (brute force, dictionary)
1. Brute Force Attack
How it works:
Tries all possible character combinations until the correct password is found.

Variants:

Pure brute-force: No shortcuts, checks every possible password.

Incremental brute-force: Starts with shorter combinations, increasing length.

Strength: Works on any password given enough time.

Weakness: Time and computing power grow exponentially with password length.

Defense: Long, random passwords; account lockouts; MFA.

2. Dictionary Attack
How it works:
Uses a predefined list of likely passwords — often common words, leaked passwords, or wordlists like rockyou.txt.

Speed: Much faster than brute-force for weak, word-based passwords.

Example:
Tries password, iloveyou, qwerty, admin123.

Defense: Avoid dictionary words; add randomness and length.

3. Hybrid Attack
How it works:
Combines dictionary and brute-force — takes dictionary words and applies variations like numbers, symbols, or capitalization.

Example:
From password → tries Password1, P@ssword2025, p@ssw0rd.

Defense: Avoid predictable substitutions; use passphrases or random strings.

4. Credential Stuffing
How it works:
Uses username/password pairs from previous breaches to try on other sites.

Reason: Many users reuse passwords across services.

Example:
If your old email and password from a gaming site are leaked, attacker tries them on Gmail or PayPal.

Defense: Use unique passwords per site; enable MFA; monitor for breaches.

5. Reverse Brute Force
How it works:
Attacker picks one common password and tries it on many different usernames/accounts.

Example:
Uses 123456 or password1 on thousands of accounts.

Defense: Don’t use common passwords; enforce password policies.

6. Phishing Attack
How it works:
Tricks users into entering their password on a fake login page or giving it via email/phone.

Method: Fake websites, spoofed emails, or social engineering.

Defense: Verify URLs, don’t click suspicious links, use phishing-resistant MFA (security keys).

7. Keylogging
How it works:
Malware or hardware logs keystrokes as the user types, capturing passwords.

Example:
Malicious software installed through phishing or infected downloads.

Defense: Keep software updated, use antivirus, avoid suspicious files, use password managers (auto-fill).

8. Shoulder Surfing
How it works:
Physically watching someone type their password.

Example:
Looking over someone’s shoulder in a public place or capturing it via security cameras.

Defense: Shield your screen/keyboard, use on-screen keyboard for sensitive entries.

9. Social Engineering
How it works:
Manipulating people into revealing passwords by exploiting trust or urgency.

Example:
Pretending to be IT support asking for login details.

Defense: Verify identities before sharing information, follow security policies.

10. Rainbow Table Attack
How it works:
Uses precomputed tables of hashes to reverse-engineer passwords from hashed values.

Defense: Use salted password hashing (bcrypt, scrypt, Argon2).

11. Man-in-the-Middle (MITM) Attack
How it works:
Intercepts communication between user and service to capture credentials.

Example:
On unsecured public Wi-Fi, attacker intercepts login requests.

Defense: Use HTTPS, VPN, and avoid logging in over public networks.

12. Password Spraying
How it works:
Tests a small set of very common passwords against many accounts to avoid detection.

Example:
Tries Spring2025! or Welcome1 across thousands of accounts.

Defense: Require strong passwords; monitor failed login attempts.

STEP 8- Summarize how password complexity affects security.

Password complexity affects security by making it harder for attackers to guess or crack the password.
Longer passwords with a mix of uppercase, lowercase, numbers, and symbols greatly increase the number of possible combinations, which slows down brute-force and dictionary attacks.
Randomness and length are more important than clever substitutions, and unique passwords for each account prevent credential reuse attacks.

