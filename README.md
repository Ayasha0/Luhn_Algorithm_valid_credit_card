# Luhn_Algorithm_valid_credit_card
This code is actually implementing the Luhn Algorithm, which is the standard checksum formula used to validate credit/debit card numbers.
Luhn Algorithm (Card Number Validation)

The Luhn Algorithm (also known as the modulus 10 or mod 10 algorithm) is a simple checksum formula used to validate a variety of identification numbers such as credit card numbers, IMEI numbers, and government IDs. It was created by IBM scientist Hans Peter Luhn in 1954 and is still widely used today in financial and security systems.

🔎 How it works:

Start from the rightmost digit of the number and move left.

Double every second digit (the even-positioned ones from the right).

If doubling results in a two-digit number (e.g., 12), add the digits together (1 + 2 = 3).

Add all the digits together (both the unchanged odd-position digits and the processed even-position digits).

If the total sum is divisible by 10, the number is considered valid; otherwise, it’s invalid.

 Example:

Card Number: 4111 1111 4555 1141

Step 1 (reverse & split): process digits as odd/even from the right.

Step 2 (apply Luhn’s rule):

Odd digits sum = 16

Even digits (doubled & adjusted) sum = 34

Total = 16 + 34 = 50

Since 50 % 10 == 0, the number is valid.

🚀 Applications:

Credit/Debit card number validation

IMEI (mobile devices) validation

Government-issued IDs (e.g., SSNs in some countries)
