# actions-training-notes
TODO:
Create an action

## Before the training

Initialize the following repositories:

https://github.com/ps-actions-sandbox/demo-workflow-syntax in your own account

https://github.com/ps-actions-sandbox/demo-environments-secrets in the enterprise account https://github.com/EficodeRND 

https://github.com/ps-actions-sandbox/demo-workflow-templates in EficodeRND

https://github.com/ps-actions-sandbox/.github in EficodeRND



# During
Make sure that you open up the presentation in presenter mode.

First thing:
https://github.com/sofusalbertsen/Actions-fundamentals
Make them go into the issues there.


https://docs.github.com/en/actions/creating-actions/about-custom-actions

https://github.blog/changelog/2021-11-10-github-actions-input-types-for-manual-workflows/ 

1. Demo

- basic workflow https://github.com/sofusalbertsen/demo-workflow-syntax 

1. Hands on:
https://github.com/ps-actions-sandbox/ActionsFundamentals

Break:
https://vclock.com/set-timer-for-15-minutes/

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

https://github.com/octokit



- github action marketplace https://github.com/marketplace?type=actions

- Github action documentation 

