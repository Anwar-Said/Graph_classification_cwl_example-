# GC_toxicity Workflow Description 
The following description will tell the user how to prepare and execute the workflow for a succesfull
repreat of the original experiment.

## Environment
For the execution environment, you are going to need a linux based machine with [cwltool](https://github.com/common-workflow-language/cwltool)
installed on it. Additionally, you will also need [docker](https://docs.docker.com/engine/install/) installed to be able to run
the containerized computing elements.

## Description

### GC_toxicity


### Required inputs
 - FileInput : 


### Generated outputs
 - result : 


## Execution
To run the workflow, you need to give the following command:
```
cwltool --no-match-user --no-read-only --preserve-environment LEAP_CLI_DIR GC_toxicity.cwl.json --FileInput data/dataset.pkl
```