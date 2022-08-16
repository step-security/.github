<p align="left">
  <img src="https://step-security-images.s3.us-west-2.amazonaws.com/Final-Logo-06.png" alt="Step Security Logo" width="340">
</p>

## Produce Software With Confidence

### [Harden Runner](https://github.com/step-security/harden-runner)

Harden-Runner GitHub Action installs a security agent on the GitHub-hosted runner (Ubuntu VM) to

1. Prevent exfiltration of credentials
2. Detect compromised dependencies and build tools
3. Detect tampering of source code during build

### [Secure Workflows](https://github.com/step-security/secure-workflows)

Automated security fixes that get you a higher OpenSSF Scorecard score.

Automatically enable security features in GitHub Actions workflow files:
1. Set minimum `GITHUB_TOKEN` permissions 
2. Pin Actions to a full length commit SHA
3. Add Step Security Harden Runner GitHub Action 

[OSSF Scorecards](https://opensource.googleblog.com/2020/11/security-scorecards-for-open-source.html) recommends using [StepSecurity's online tool](https://app.stepsecurity.io/) for [#1](https://github.com/ossf/scorecard/blob/main/docs/checks.md#token-permissions) and [#2](https://github.com/ossf/scorecard/blob/main/docs/checks.md#pinned-dependencies). 

