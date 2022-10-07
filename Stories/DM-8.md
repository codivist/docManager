# DM-8

## CI/CD setup for new feature

### Magnitude 5

#### Description
As per RimSys CI/CD standards, this new feature must automagically use the pipelines for delivering updates from github to Dev, Staging and Production servers.

#### Value
CI/CD processes keep our company ahead of competitors and our users happy.

#### Acceptance Criteria
* When the github pipeline for the `development` branch succeeds the `development` branch will be pushed to the dev server: `https://dev.example.test`
* Pipeline for the `staging` branch will push to: `https://staging.example.test`
* Pipeline for the `main` branch will push to our production site: `https://example.com`

At this point the existing Kubernetes (K8s) will automagically recycle the correct server and our new code will be live and ready for testing or production.

#### Notes
Most of this process is already set up, but setting Mag:5 for any issues that might come up from this new feature

[Back to Overview](../readme.md)