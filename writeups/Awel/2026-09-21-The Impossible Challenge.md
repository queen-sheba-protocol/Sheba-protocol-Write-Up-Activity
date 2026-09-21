# The Impossible Challenge

**Author:** Awel Abduljelil
**Date:** 2026-09-21
**Category:** Cryptography / Steganography
**Source:** TryHackMe
**Difficulty:** Medium

## Summary

The Impossible Challenge is a cryptography and steganography challenge involving ROT13, ROT47, Hex, Base64, and Unicode zero-width characters.

## Background

The challenge provides an encoded ciphertext and a password-protected ZIP file containing `flag.txt`.

## Steps to Reproduce

1. Download the provided ZIP file and confirm that it requires a password.
2. Decode the provided ciphertext using CyberChef with:

   ```text
   ROT13 → ROT47 → Hex → Base64
   ```
3. The decoded message says:

   ```text
   It's inside the text, in front of your eyes!
   ```
4. Inspect the webpage and notice unusual characters hidden inside the `Hmm` title text.
5. Copy the `Hmm` text and decode it using a Unicode steganography tool.
6. The hidden message reveals the ZIP password.
7. Use the password to extract `flag.txt` and read the flag.

## Root Cause

The challenge hides information using Unicode zero-width characters. These characters are invisible but can store additional data inside normal-looking text.

## Impact

In real-world applications, invisible Unicode characters could be used to hide information in documents, messages, websites, or other text-based content.

## Remediation

* Detect unexpected zero-width characters.
* Normalize Unicode input where appropriate.
* Validate and sanitize user-controlled text.
* Use Unicode-aware security analysis tools.

## Lessons Learned

* Do not rely only on what is visually displayed.
* Inspect webpage elements when a clue points to hidden text.
* Learn common encoding techniques such as ROT13, ROT47, Hex, and Base64.
* Invisible Unicode characters can be used for steganography.

### Flag

```text
THM{Zero_Width_Characters_EZPZ}
```
