# gh-first-workflow

This repository has an example of workflow to get started on github actions.

```yaml
name: First Workflow Example
on: workflow_dispatch
jobs:
  greeting-job:
    runs-on: ubuntu-latest
    steps:
      - name: Print hello world
        run: |
          echo "Hello World !"
      - name: Print Bye
        run: |
          echo "Done - Bye !"
```

`workflow_dispatch` means the workflow can be executed manually. A workflow can be defined for a repository. In a single repository, there can be multiple workflows.

There can be multiple jobs in a workflow. In this example, we have a `greeting-job` job which runs on `ubuntu`. There are two steps in this job: (1) Prints "Hello World !" and (2)
Prints "Done - Bye !"
