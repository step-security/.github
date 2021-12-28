<p align="left">
  <img src="https://step-security-images.s3.us-west-2.amazonaws.com/Final-Logo-06.png" alt="Step Security Logo" width="340">
</p>

## Thwart software supply chain attacks

### [Harden Runner](https://github.com/step-security/harden-runner)

Harden the Ubuntu VM on which GitHub Actions runs your workflow: 

1. Install agent using a step in the workflow. Step takes less than 5 seconds to run  
    ```
      - name: Harden Runner
        uses: step-security/harden-runner@v1
        with:
          egress-policy: audit
    ```
2. Discover outbound traffic 
3. Restrict outbound traffic, prevent DNS exfiltration, and exfiltration of credentials    
4. Detect unauthorized modification to source code or dependencies 
5. Cryptographically verify tools downloaded and used as part of the pipeline

Workflows using harden-runner:
1. https://github.com/nvm-sh/nvm/tree/master/.github/workflows
2. https://github.com/shivammathur/setup-php/blob/master/.github/workflows/node-release.yml


### [Secure Workflows](https://github.com/step-security/secure-workflows)

Automatically enable security features in GitHub Actions workflow files:
1. Set minimum `GITHUB_TOKEN` permissions 
2. Pin Actions to a full length commit SHA
3. Add Step Security Harden Runner GitHub Action 

#1 and #2 are [recommended by GitHub](https://docs.github.com/en/actions/security-guides/security-hardening-for-github-actions) and get you a higher [Scorecards](https://github.com/ossf/scorecard) score. 

### [Supply Chain Goat](https://github.com/step-security/supply-chain-goat)

Supply Chain Goat follows the tradition of existing *Goat projects (e.g. [OWASP Web Goat](https://github.com/WebGoat/WebGoat)) that provide
a training ground to practice implementing countermeasures specific to the software supply chain. 

1. Learn about past supply chain incidents
2. Hands-on tutorials for countermeasures
3. Understand why countermeasures are needed