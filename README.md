# actions-training-notes


## Before the training

Check if new version of the slides have been uploaded:
https://github.com/ps-resources/es-offerings-assets/tree/main/gh-actions-fundamentals


Initialize the following repositories:
https://github.com/ps-actions-sandbox/demo-workflow-syntax in your own account

https://github.com/ps-actions-sandbox/ActionsFundamentals
Create a repo from that template and make them go into the issues there.

Documentation
https://docs.github.com/en/actions

# Day 1
Make sure that you open up the presentation in presenter mode.

Make them go into the templated repo (Actions fundamental)

1. Demo
- basic workflow https://github.com/sofusalbertsen/demo-workflow-syntax 


1. Hands on:
https://github.com/ps-actions-sandbox/ActionsFundamentals
Make them create a repo from that template and use the hol

Actions:
Starter repos
- Container: https://github.com/actions/container-action
- Javascript: https://github.com/actions/javascript-action

Break:
https://vclock.com/set-timer-for-10-minutes/
https://vclock.com/set-timer-for-15-minutes/
https://vclock.com/set-timer-for-20-minutes/

2. Demo
Create your own action
* https://github.com/sofusalbertsen/custom-action
* in another repo, use this in a workflow
```yaml
      - name: Run custom action from antoher
        uses: sofusalbertsen/custom-action@main
        with:
          myInput: sofus
```

# Day 2

Demoing things from: https://github.com/EficodeDemoOrg


Environments and secrets demo:
https://github.com/EficodeDemoOrg/demo-environments-secrets/tree/main/.github/workflows
