# JFrog Platform Demo: Distribution

## Preparation

Pipelines
- Select "demo" project -> Project Settings -> Integrations -> Add an Integration
  - Distribution
    - Name: distribution
    - Integration Type: Distribution
    - Distribution URL: <auto-filled>
    - User: admin
    - API Key: <press "Get API Key">
    - Signing Key Passphrase: <leave blank (if you configure this, put it)>

- Select "demo" project -> Project Settings -> Pipeline Sources -> Add Pipeline Source -> From YAML
  - Branch Type: Single Branch
  - Protocol Type: HTTPS
  - Name: jfrog_demo_distribution
  - SCM Provider Integration: github
  - Repository Full Name: tsuyo/jfrog-demo-distribution
  - Branch: main
  - Pipeline Config File Filter: pipelines/pipelines-.+.yml
