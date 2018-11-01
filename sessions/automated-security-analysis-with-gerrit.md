# Automated Security Analysis with Gerrit Robot Comments

Gerrit Code Review is often used for enforcing security and compliance with
opensource components, thanks to its ability to require special review workflows
when the project's dependencies are modified.

That process is typically managed by special "reviewers" that manually check
and approve or reject changes using special "Library Compliance" labels.
What if we had a system that automatically checks for those issues, removing
the requirement of this tedious and error-prone task, while allowing developers
to focus on more important tasks?

This talk is about showing an approach where you can see how this can be
automated out of the box using Jenkins / GerritHub DevOps pipeline, with
the aid of the Meterian engine. We will also  leverage Gerrit's Robot Comments
to streamline the whole process of detecting, notifying and fixing common
security and compliance issues.

*[Bruno Bossola, CTO / meterian.io](../speakers.md#bbossola)*
