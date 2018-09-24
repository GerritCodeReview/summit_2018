# Different change workflows in Gerrit

In Release 2.3 (2012) draft changes and draft patch set workflow
was added to Gerrit. This implementation extended change status with
DRAFT value. DRAFT status in change occurs before NEW and will be for
a change that is not meant for review (yet). Draft changes and draft
patch sets can be removed or published. Publishing a draft patchset in
a draft change irreversibly upgrades the change status to NEW. In addition
draft changes implied visibility restriction: only change owners and
reviewers can see drafts.

In 2013 OpenStack project proposed alternative Work In Progress workflow,
that was not adopted in gerrit core at that time. Later, based on his work,
work in progress plugin was created. This plugins had some limitation because
it wasn't a core feature, like set-Ready, set-WIP events were not fired or
suppressing mail notifications for WIP changes wasn't implemented.

In 2017, during migration of Chromium project from Rietveld to Gerrit the WIP
workflow got another momentum, as it was a hard requirement for Chromium project
migration to Gerrit.

In 2.15 Work In Progress workflow was added to Gerrit core and Draft changes
workflow was discontinued.

In this talk we will compare different workflows and possible alternatives and
clarify the migration path from older Gerrit versions that may still have
draft changes and draft patch sets. We will also look at possible improvements
of new WIP workflow.

*[David Ostrovsky, Gerrit Maintainer](../speakers.md#davido)*