# Password-strength-checker
Understand what makes a password strong and test it against password strength tools.

This repository contains tools and examples to **generate strong passwords** and **evaluate password strength** with a simple, explainable meter. 
It's intended for educational use — to learn what makes a password strong and to experiment in a safe way.

## Contents
# Password Strength - Scoring Explanation

The simple meter included in this repo uses the following factors to estimate strength:

1. **Length**: longer passwords increase entropy roughly linearly.
2. **Character variety**: presence of lowercase, uppercase, digits, symbols increases the character pool.
3. **Entropy estimate**: estimated bits = length * log2(pool_size) where pool_size is estimated from categories present.
4. **Common patterns penalty**: repeated sequences, common substrings (like 'password', '1234', 'qwerty'), keyboard walks, or years degrade strength.
5. **Score bucket**: meter maps bits-of-entropy and penalties to a 0-4 score (Very Weak to Very Strong).

## Recommendations
- Use at least 12 characters for user-generated passwords; 16+ for high-value accounts.
- Prefer passphrases: multiple unrelated words are easier to remember and can offer high entropy.
- Use a password manager for unique strong secrets per site.


## Tools
https://www.passwordmonster.com/

## Safety
- Do not paste real, production passwords into third-party web pages or services.
- Use this repo for education; integrate into workflows carefully.
