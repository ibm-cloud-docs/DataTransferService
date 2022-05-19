# Data Transfer Service docs
{: #readme}

This repository stores documentation source files for the Data Transfer service.

- [Jenkins build](https://wcp-ace-docs-jenkins.swg-devops.com/job/Docs-build/job/Docs-build-DataTransferService/)
- Slack channel: `#docs-datatransferserv`

## Publishing

Start in the `staging` branch of this repository. Commits to `staging` run a build, lint your content, and publish changes to the [IBM Cloud stage docs](https://test.cloud.ibm.com/docs/infrastructure/DataTransferService). After you're happy with the changes, copy the modified files to the [IBM-Bluemix-Docs/DataTransferService](https://github.com/IBM-Bluemix-Docs/DataTransferService) repository, and then validate the changes in the [IBM Cloud production docs](https://cloud.ibm.com/docs/infrastructure/DataTransferService).

### Staging

1. Commit to `staging`. Check that [the build](https://wcp-docs-team-jenkins.swg-devops.com/job/build/job/cloud-docs/job/DataTransferService/) passes linting. 
2. Validate your changes in [staging](https://test.cloud.ibm.com/docs/DataTransferService).

### Production

1. Work in `staging` branch until you're happy with the changes. 
2. Merge the changes to the `production` branch.
3. After the merge, validate your changes in [production](https://cloud.ibm.com/docs/DataTransferService).
