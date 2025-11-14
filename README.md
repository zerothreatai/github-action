# Zero Threat AI Powered Security Scanner

Secure your code proactively. Use the ZeroThreat AI Powered Web Application/API Security Scanner to perform Dynamic Application Security Testing (DAST). It enables comprehensive Dynamic Application Security Testing (DAST) to detect vulnerabilities, making findings readily available on the ZeroThreat Portal for review.

## Inputs

| Input               | Description                                                          | Required | Default |
| ------------------- | -------------------------------------------------------------------- | -------- | ------- |
| `ZT_TOKEN`          | ZT_TOKEN to authenticate API request & start the scan.               | Yes      |         |
| `WAIT_FOR_ANALYSIS` | Set this true to wait for analysis to complete before finishing job. | No       | false   |
| `ON_PREM_PROXY_API_URL` | Set proxy url host to scan internal targets. | No       |    |


## How It Works

1. **ZeroThreat AI Scanner**: The DAST scan is triggered by passing the `zt_token`. Each token corresponds to a specific target defined within the ZeroThreat application. Upon receiving the token, the ZeroThreat DevOps Bot executes prerequisite checks before commencing the scan process.
2. **Scan Report**: As soon as the ZeroThreat DevOps Bot starts the security scan, The scan report will be available in the ZeroThreat Portal.

### Secrets Setup
1. Generate the `zt_token` from the ZeroThreat Portal.
   
2. Add the secret in your GitHub repository under **Settings > Secrets**:
    - `zt_token`: ZT_TOKEN to authenticate API request & start the scan.


## Notes

- Ensure secrets are correctly configured in your GitHub repository for scan initiation. 
- ZeroThreat offers a centralized dashboard displaying all scan results.

