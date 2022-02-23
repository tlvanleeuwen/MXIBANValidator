# Description
This module adds a validation rule and java action that validates the structure of an IBAN string according to the ISO/IEC 7064 standard. Please note that this module does not check whether the IBAN exists, it only validates whether it is a valid IBAN number using the check digit code.

This module should work with all IBAN account numbers over the world, but has mostly been tested with Dutch IBAN account numbers. So let me know when there are exceptions that I can add to this module!

For more information on how the IBAN is checked, please read the following Wikipedia page about this standard: https://en.wikipedia.org/wiki/International_Bank_Account_Number#Validating_the_IBAN.

# Typical usage scenario
This module can be used to validate user input of an IBAN bank account number, and should prevent most typo errors (the check digit code should correspond to the rest of the IBAN number).

# Features and limitations
- This module holds a Java action that returns a boolean when the IBAN is correctly validated and a validation rule that can be used in a decision in your own logic.

- This module does not validate whether the IBAN account number actually exists. It only checks whether the IBAN number is correctly structured.
