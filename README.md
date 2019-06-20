# Data Transfer Service docs
This repository stores documentation source files for the Data Transfer service.

- [Jenkins build](https://wcp-ace-docs-jenkins.swg-devops.com/job/Docs-build/job/Docs-build-DataTransferService/)
- Slack channel: `#docs-datatransferserv`

## Publishing

Start in the `staging` branch of this repository. Commits to `staging` run a build, lint your content, and publish changes to the [IBM Cloud stage docs](https://test.cloud.ibm.com/docs/infrastructure/DataTransferService). After you're happy with the changes, copy the modified files to the [IBM-Bluemix-Docs/key-protect](https://github.com/IBM-Bluemix-Docs/DataTransferService) repository, and then validate the changes in the [IBM Cloud production docs](https://cloud.ibm.com/docs/infrastructure/DataTransferService).

### Staging

1. Commit to `staging`. Check that [the build](https://wcp-ace-docs-jenkins.swg-devops.com/job/Docs-build/job/Docs-build-DataTransferService/) passes linting. 
2. Validate your changes in [staging](https://test.cloud.ibm.com/docs/infrastructure/DataTransferService).

### Production

1. Work in `staging` branch until you're happy with the changes. 
2. Copy the changes to the [IBM-Bluemix-Docs/key-protect](https://github.com/IBM-Bluemix-Docs/DataTransferService) repository.

    **Note:** To publish changes externally, you need to use a public GitHub account. After you create an account, fork the repository, and then open a pull request to propose changes.

2. After the pull request is merged, validate your changes in [production](https://cloud.ibm.com/docs/infrastructure/DataTransferService).
    

