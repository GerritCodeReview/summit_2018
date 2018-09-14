# Propose a talk about Gerrit Code Review

The User Summit is about people and their experiences
in using Gerrit Code Review for their teams and companies.

We are looking forward to receiving fantastic proposals from industry
experts about how they have used and improved their Development
Pipeline and/or have extended Gerrit with amazing plugins.

Your experience could include as well the entire Continuous
Integration pipeline, including integration with CI (Jenkins or others)
and your issue tracking system.

## How to submit my proposal?

It is very simple, just clone the ```summit/2018``` repository and add your session
to the schedule:

1. Create a Markdown under the /sessions directory using the template.md as an example
2. (Optional) Link your session into the schedule.md on the date/time you would like to present
3. Push your changes for review to gerrit.googlesource.com/summit/2018

__NOTE:__ You need to be registered on https://gerrit-review.googlesource.com in order
to be able to be authorized to push changes for review.

**Example:**

```bash
$ git clone https://gerrit.googlesource.com/summit/2018 && (cd 2018 && curl -Lo `git rev-parse --git-dir`/hooks/commit-msg https://gerrit-review.googlesource.com/tools/hooks/commit-msg ; chmod +x `git rev-parse --git-dir`/hooks/commit-msg)
$ cd 2018/sessions
$ cp template.md myamazingtalk.md
$ vi myamazingtalk.md

...

$ git add myamazingtalk.md & git commit -m 'This is my amazing talk'
$ git push origin HEAD:refs/for/master
```

## How my talk is going to be voted and selected?

The voting is opened to everyone that is registered to
https://gerrit-review.googlesource.com.
People will be able to post comments, ask questions and vote for it.

The top 13 rated proposals will become part of the Gerrit User Summit 2018
schedule.

## Will my talk be recorded and published?

We can record the full session and publish it for allowing other people
to watch it online later on, even if they have not attended the Summit.
However, if you do not wish to be recorded, just let us know and include
a simple note in your talk proposal.

You will still be free to publish your slides anywhere on the web
and we will just point to them.
