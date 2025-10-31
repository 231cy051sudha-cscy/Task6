# Task6
Objectives
Learn what factors (length, character sets, structure) most strongly affect password strength.
Compare passwordmeter.com feedback across passwords of varying complexity.
Check whether any tested password has appeared in public breaches.
Produce an evidence-backed set of best practices for choosing passwords.

Tools & safety notes
passwordmeter.com — heuristic-based password strength checker. Useful for quick feedback on length/variety/sequences but not an absolute measure of resistance to sophisticated attacks.
Have I Been Pwned — Pwned Passwords — checks if a password has appeared in known breach dumps. Use the k-anonymity API or the web interface — do not paste real password into untrusted sites. (You used the reputable service.)
Safety reminder: Do not publish or share real passwords in public. In any report or screenshot, redact the exact password; show only structure (e.g., Upper+Lower+Digit+Symbol, len=8).

Step-by-step procedure you followed (detailed)
Step 1 — Plan & Scope
Defined the purpose: evaluate how length and character variety affect strength and whether passwords are in breach lists.
Set metrics to record: password structure (redacted in shared reports), length, character classes used, entropy estimate, passwordmeter score & textual feedback, and pwned-status.

Step 2 — Create password candidates
created several passwords covering a range of complexity. Example categories (do not store raw passwords in reports):
Very weak — lowercase only, short (e.g., lowercase, len=8)
Weak — mixed case, short (e.g., Upper+Lower+Digit, len=9)
Medium — mixed + symbols (e.g., Upper+Lower+Digit+Symbol, len=9)
Strong (passphrase) — multiple words (e.g., 4-word passphrase)
Very strong (random) — long random string (e.g., random chars, len=12+)

Step 3 — Test on passwordmeter.com
For each password:
Open passwordmeter.com in your browser.
Enter the password (if documenting, enter a structurally identical but redacted string).
Record the score (e.g., 100% / Very Strong), the additions/deductions table, and any suggestions (like “add more characters”, “avoid common words”).
Note whether deductions occur (sequential characters, repeated characters, letters-only, numbers-only, etc.).

Breach check (Have I Been Pwned)
For each password:
Use Have I Been Pwned’s Pwned Passwords page or the k-anonymity API.
If using the web UI, paste only into the official site. If using the API, use the k-anonymity flow (hash prefix) to avoid exposing the full password.
Record whether the password appears in breach lists and, if shown, how many times.

make them as csv sheet 
(Redacted) password structure / ID
length
char sets used
entropy (bits)
passwordmeter score & feedback
pwned result (yes/no & count if provided)
notes / interpretation
conclusion & analysis :
Compare how scores changed with length vs. with symbols.
Check whether any “very strong” results still appeared in breach lists.
Translate findings into practical recommendations.
