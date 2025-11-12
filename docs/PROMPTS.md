# Prompts

## Make a plan

Here is our job for today: creating a document `docs/PLAN.md`. No implementation yet, just a plan. The goal is to (a) write a docker compose setup that at runtime mounts the source, builds the mkdocs site and serves it. I want to serve it using `nginx` for speed. (b), create a tool link_check/link_check.py which should spider the site as served in Docker, and verify every non-external link, reporting back on any 404s. The report should be in yaml, and map the page to any broken links. Also verify the nav itself: if any links presented by the nav are broken, report those, too. First, carefully construct a detailed plan for (a) and (b), considering how we can iterate and especially test each step. 

- Create a separate mkdocs site that we can use for testing the Docker set-up as we're implementing, as building the full site can take up to 30 minutes. Make sure the plan covers this aspect: `test-docs/`. 

- Consider performance implications for (b). Note CAREFULLY, considering the implications: as we're always running against a local Docker container, we're compute bound, NOT IO bound: we want multiple processes, not asyncio. Fast, concise, simple to understand and correct. 

## Review docs/PLAN.md carefully!

## Make a TODO

Write a detailed document `docs/TODO.md`, derived from `docs/PLAN.md` which breaks the plan into task-sized chunks of a suitable granularity that can be tested in isolation.

## Review docs/TODO.md carefully!

## Make Epics and Issues

From `docs/TODO.md`, instruct the git-github-operator agent to create two Epic issues: one for the serving, and one for the link checking. They should each clearly state the scope (from the TODO and or PLAN), and list a set of sub-tasks, with check boxes, linking to issues you create for each task. Create issues in implementation order. Label the epics with the 'epic' label, and explicitly reference the PLAN.md and TODO.md documents, with links. Each issue should reference the #id of the Epic they form part of.

## Clear!

```
/clear
```
