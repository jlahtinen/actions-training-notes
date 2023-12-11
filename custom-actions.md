https://github.com/actions/container-action

All the different actions are listed here:
https://github.com/actions

A custom actions has inputs and outputs, and runs, where the steps are defined.
Both JS and Docker actions have one step to perform, while composite actions can have multiple steps.
All of them can have abitrary number of inputs and outputs.

https://docs.github.com/en/actions/creating-actions/creating-a-javascript-action


Composite action:
https://github.com/actions/upload-pages-artifact/blob/main/action.yml


name: my-first-workflow
on: [workflow_dispatch]
jobs:
  hello-world:
    runs-on: ubuntu-latest
    steps:
      - name: output hello world
        run: echo hello world
      - name: show github context
        run: echo '${{ toJSON(github)}}'
      - uses: sofusalbertsen/custom-action@main
        with:
          myInput: "sofus"