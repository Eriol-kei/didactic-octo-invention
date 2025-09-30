# didactic-octo-invention
Understand what makes a password strong and test it against password strength tools

## Objective
Understand what makes a password strong and evaluate multiple examples using an online password strength checker (e.g., [passwordmeter.com](https://passwordmeter.com)).

---

## Methodology
1. Created multiple test passwords with varying complexity (weak → strong).
2. Tested each password on the online strength checker.
3. Recorded tool scores, feedback, and computed entropy.
4. Compared results to identify best practices for strong password creation.
5. Researched common password attacks and summarized findings.

---

## Passwords Tested
*(Note: For security, actual passwords are masked in this report. Only characteristics are shown.)*

| ID | Example (masked) | Length | Char Types Used | Tool Score | Tool Feedback | Entropy (bits) | Notes |
|----|------------------|--------|-----------------|------------|---------------|----------------|-------|
| P1 | `s*****e`        | 7      | lowercase       | 8 / 100   | Too short; dictionary word | 33.2 | Very weak |
| P2 | `s*******2`      | 9      | lowercase+digits | 18 / 100  | Add uppercase/symbols | 53.6 | Weak |
| P3 | `S*******2`      | 9      | mixed+digits    | 24 / 100   | Good — increase length | 59.5 | Medium |
| P4 | `S******!3`      | 12     | mixed+digits+symbol | 78 / 100 | Strong — add more length | 78.6 | Strong |
| P5 | `c************y` | 20     | lowercase+hyphen (passphrase) | 65 / 100 | Uses common words | 94.5 | Good, but dictionary-based |
| P6 | `G**********z`   | 16     | upper+lower+digits+symbols | 92 / 100 | Excellent | 100.9 | Very strong |
| P7 | `A****@9090<>`  | 16     | mixed+digits+symbols | 100 / 100 | Excellent balance | 95.3 | Strong & memorable |

---

## Key Learnings & Best Practices
- **Length is critical:** longer passwords resist brute-force exponentially better.
- **Mix character sets:** use uppercase, lowercase, digits, and symbols.
- **Avoid dictionary words:** attackers use dictionaries and common substitutions (`P@ssw0rd`).
- **Passphrases work well:** multiple unrelated words + symbols/numbers = strong and memorable.
- **Never reuse passwords:** use unique passwords for each account.
- **Use a password manager:** to store and generate random high-entropy passwords.
- **Enable MFA:** adds strong protection even if a password is compromised.

---

## Common Password Attacks
- **Brute Force:** tries all possible combinations; strength depends on entropy and length.
- **Dictionary Attacks:** guesses words and common variations.
- **Credential Stuffing:** reuses leaked username/password combos across sites.
- **Rainbow Tables:** precomputed hash lookups (mitigated by salted hashing).

---

## Conclusion
- The **random 16-character password (P7)** achieved the highest tool score and entropy.  
- The **passphrase (P5)** was strong but penalized due to dictionary words.  
- The most **practical balance** is a passphrase with mixed classes (e.g., P7) combined with a password manager and MFA.  
- Password strength improves most significantly with **length + randomness**, not just character variety.  

---

## Appendix
- Tool used: [PasswordMeter.com](https://passwordmeter.com)   
- Entropy calculation reference: [Wikipedia - Password Strength](https://en.wikipedia.org/wiki/Password_strength) 
