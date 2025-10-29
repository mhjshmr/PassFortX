# PassFortX – Password Strength Checker & Generator

PassFortX is a Python-based cybersecurity tool designed to evaluate password strength, estimate cracking time, and generate secure random passwords.
It demonstrates key password security principles, helping users understand how to create strong and resilient credentials.
<br><br>

<div align="center">
  <img src="https://github.com/mhjshmr/PassFortX/blob/main/passfortx.png?raw=true" alt="PassFortX Screenshot" width="400">
</div>

## Overview

PassFortX provides two primary features:
1. **Password Strength Analysis** – Evaluates password security based on length, complexity, character variety, and common password patterns.
2. **Secure Password Generation** Creates cryptographically secure passwords suitable for modern security standards.

## Features

### Password Strength Checker
- Evaluates password length and character complexity.
- Checks against a list of common passwords.
- Assesses character variety (uppercase, lowercase, numbers, symbols).
- Estimates brute-force cracking time.

### Password Generator
- Generates cryptographically secure random passwords.
- Allows customizable password length.
- Includes a mix of uppercase, lowercase, numbers, and special characters.
- Automatically assesses generated password strength.

## Getting Started

### Prerequisites
- Python 3.x installed on your system

### Installation

1. Clone this repository or download the files:
```bash
git clone https://github.com/mhjshmr/PassFortX.git
cd PassFortX
```

2. No additional dependencies required - uses Python standard library only!

### Usage

Run the program:
```bash
python PassFortX.py
```

Follow the interactive menu:
1. **Check a password** - Enter any password to analyze its strength
2. **Generate a password** - Create a secure random password
3. **Exit** - Close the program

## Examples

### Example 1: Checking a Weak Password
```
Enter your password: password123

Password Strength:  Weak (common password)
Estimated time to crack: 0.52 seconds
```

### Example 2: Checking a Strong Password
```
Enter your password: MyS3cur3P@ssw0rd!

Password Strength:  Strong
Estimated time to crack: 2.3e+15 years
```

### Example 3: Generating a Password
```
Enter desired password length (default 12): 16

Generated password: K9#mL@pQ2xR$nF7v
Password Strength: Strong
Estimated time to crack: 8.7e+18 years
```

## How It Works

### Strength Analysis Criteria:
1. **Length** – Less than 6 characters: Weak; 6–7 characters: Medium; 8+ characters with complexity: Strong
2. **Character Variety** – Lowercase, uppercase, numbers, special characters
3. **Common Password Check** – Flags passwords found in common password lists
4. **Crack Time Estimation** – Calculates possible combinations based on character types, assuming one billion attempts per second

### Password Generation:
- Randomly selects characters from all categories
- Ensures all character types are included
- Shuffles characters to improve unpredictability
  
## Best Practices

- **Use at least 12 characters** - Longer is always better  
- **Mix character types** - Combine uppercase, lowercase, numbers, and symbols  
- **Avoid common passwords** - Never use "password123", "qwerty", etc.  
- **Use unique passwords** - Different password for each account  
- **Consider a password manager** - Safely store complex passwords  

## Security Considerations

- The tool provides estimates based on brute-force attacks; real-world attacks may use more sophisticated methods.
- Weak passwords are typically short, predictable, or common.
- Always complement strong passwords with multi-factor authentication (2FA) and approved security practices.

## Technical Details

- **Language** - Python 3.x
- **Standard Library Modules:** - `random`,`string`
- **Core Functions:** 
   - `check_strength(password)` – Evaluates password strength
   - `generate_password(length)` – Produces a secure random password
   - `crack_time_estimate(password)` – Estimates brute-force cracking time


## References

- [OWASP Password Guidelines](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)
- [NIST Password Standards](https://pages.nist.gov/800-63-3/sp800-63b.html)
- [How Secure Is My Password?](https://www.security.org/how-secure-is-my-password/)

**Stay secure! **
