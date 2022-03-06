<p align="left">
  <img src="https://step-security-images.s3.us-west-2.amazonaws.com/Final-Logo-06.png" alt="Step Security Logo" width="340">
</p>

## Thwart software supply chain attacks

StepSecurity defines a supply chain attack as an attack that tries to hijack software that you produce or consume. StepSecurity provides a holistic understanding of software supply chain security issues and how they can be prevented with the following leading-edge components that can be implemented in many GitHub repositories to counter these types of threats and lack of detection.

### [Harden Runner](https://github.com/step-security/harden-runner)

This GitHub Action can be used to visualize process, file, and network activity from GitHub-hosted runners in a Web UI. It can also be used to restrict outbound traffic to allowed endpoints.

Hijacked dependencies and compromised build tools typically make outbound requests during the build process to exfiltrate data or credentials. This was the case in the [Codecov breach](https://www.bleepingcomputer.com/news/security/popular-codecov-code-coverage-tool-hacked-to-steal-dev-credentials/), in the [dependency confusion attacks](https://medium.com/@alex.birsan/dependency-confusion-4a5d60fec610), and the recent [npm package hijacks](https://github.com/faisalman/ua-parser-js/issues/536).

[Harden Runner](https://github.com/step-security/harden-runner) is a first-of-its-kind patent-pending technology that automatically correlates outbound traffic with each step of a workflow. Add the recommended outbound endpoints to your workflow file, and only traffic to these endpoints will be allowed.

### [Secure Workflows](https://github.com/step-security/secure-workflows)

Automatically enable security features in GitHub Actions workflow files:
1. Set minimum `GITHUB_TOKEN` permissions 
2. Pin Actions to a full length commit SHA
3. Add Step Security Harden Runner GitHub Action 

[OSSF Scorecards](https://opensource.googleblog.com/2020/11/security-scorecards-for-open-source.html) recommends using [StepSecurity's online tool](https://app.stepsecurity.io/) for [#1](https://github.com/ossf/scorecard/blob/main/docs/checks.md#token-permissions) and [#2](https://github.com/ossf/scorecard/blob/main/docs/checks.md#pinned-dependencies). 

### [Supply Chain Goat](https://github.com/step-security/supply-chain-goat)

Supply Chain Goat follows the tradition of existing *Goat projects (e.g. OWASP Web Goat). It provides
a training ground to practice implementing countermeasures specific to the software supply chain. 

1. Learn about past supply chain incidents
2. Hands-on tutorials for countermeasures
3. Understand why countermeasures are needed
