# Elevate-Labs-Task-6

Objective -  Understand what makes a password strong and test it against password strength tools.

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
