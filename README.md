# Bash Background Jobs

## Objectives

1. Understand why this is useful
2. Create background tasks in bash
3. View currently running background tasks
4. Switch between background tasks

### Understand why this is useful

Sometimes you might only have access to a single terminal window (for example, with the Learn IDE!) and you'll want to run multiple processes. Luckily, there is an easy solution for this: Job control in bash!

This will be really helpful in the OO Student Scraper lab where you will want to run a server so you can access a locally stored website _and_ run tests that will need to access your this server.

### Create a background task in bash

If you would like a start a new process (like a local server) in the background, all you need to do as add an ` &` to the end of the command like this: `jekyll serve &`. This process will now run in the background in this terminal window.

>Note: You may have to press `enter` or `return` to get your prompt back.

### Show currently running jobs

Great, now we've got some tasks quietly running in the background, so how to we keep track of them? Simple, use the command `jobs` in your terminal to get a list of all jobs running in this window. Each job will have a job number in front of it that will look like this: `[1]`. Now we can easily keep track of all processes that are currently running.

### Switching between jobs

You can easily switch which job runs in the foreground with the `fg` command followed by the job number. So if our jekyll server is running in the background as job number 1, we can simply switch to it by doing `fg 1`. Once you've switched your process to running in the foreground you can act on it as normal (for example, you could now shut your server down with `ctrl + c`).

## Resources

 - [More Info on Bash Jobs](http://www.tldp.org/LDP/abs/html/x9644.html)

<a href='https://learn.co/lessons/bash-background-jobs' data-visibility='hidden'>View this lesson on Learn.co</a>
