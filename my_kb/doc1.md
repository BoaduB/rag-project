# Enterprise Password and Authentication Policy

## 1. Password Complexity Requirements
All corporate user accounts must enforce strict password creation rules to prevent brute-force attacks. Passwords must be at least 12 characters long and include a combination of uppercase letters, lowercase letters, numbers, and special symbols. Reusing any of the last 5 previous passwords is strictly prohibited.

## 2. Multi-Factor Authentication (MFA)
Multi-factor authentication is mandatory for all employees accessing internal company networks, cloud infrastructure, and production environments. Hardware security keys or authenticator application tokens must be utilized. SMS-based verification is deprecated due to security vulnerabilities like SIM swapping.

## 3. Account Lockout Thresholds
To mitigate automated credential stuffing attacks, user accounts will be temporarily locked out for exactly 30 minutes after five consecutive failed login attempts. System administrators can manually override and unlock accounts via the internal IAM portal.