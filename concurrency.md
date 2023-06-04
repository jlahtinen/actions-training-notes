You can use jobs.<job_id>.concurrency to ensure that only a single job or workflow using the same concurrency group will run at a time. A concurrency group can be any string or expression. Allowed expression contexts: github, inputs, vars, needs, strategy, and matrix. For more information about expressions, see "Expressions."

