# API Token and Secret Management Guidelines

## 1. Token Expiration and Rotation
API access tokens generated for internal microservices and external developer integrations must never exceed a maximum lifespan of 90 days. Automated scripts must run monthly to check for expired or compromised tokens and revoke them immediately.

## 2. Environment Variables and Hardcoding
Hardcoding API keys, database credentials, or secret tokens directly into source code repositories is a critical security violation. All sensitive configuration parameters must be loaded dynamically using environment variables or stored securely inside an encrypted secrets manager.

## 3. Rate Limiting and Monitoring
Public-facing REST API endpoints must implement strict rate limiting. Any IP address exceeding 100 requests per minute will be automatically throttled and flagged for review by the security operations center (SOC).