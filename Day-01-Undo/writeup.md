# Day 01 – Undo

**Platform:** picoCTF  
**Category:** General Skills  
**Difficulty:** Easy

### Challenge Description

"Can you reverse a series of Linux text transformations to recover the original flag?"

The challenge involved reversing multiple text transformations in the correct order to recover the original flag.

### Techniques Learned

| Transformation | Linux command |
|---|---|
| Base64 decoding | `base64 -d` |
| Reversing text | `rev` |
| Replacing dashes with underscores | `tr '-' '_'` |
| ROT13 decoding | `tr 'A-Za-z' 'N-ZA-Mn-za-m'` |

### Key Takeaway

I learned how to use basic Linux commands to decode and reverse text transformations, and why understanding the order of operations matters when solving CTF challenges.
