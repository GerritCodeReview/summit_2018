# Lessons learned from Gerrit 2.7 to 2.14 migration

At Intel connectivity division Gerrit is in the center of our
Continuous Delivery setup that supports daily work of few thousand developers. 

Gerrit is customized to automate daily work and improve the quality of our
deliveries. Many of those customizations have been done directly in the Gerrit
core based on the 2.7 version.

Recently we went through an upgrade from 2.7 to 2.14.
Apart from redesigning our customizations we had to coordinate a rollout in
the large development organization that minimizes the impact on the customer
deliveries.

We would like to share with you lessons learned from this experience.
They cover some of the technical challanges as well as other aspects that are
often forgotten like communication strategy, stakeholder alignment, documentation,
test coverage and team work.

*[Krzysztof Miesniak, Workflow Architect and Software Engineering Manager, Intel Corporation](../speakers.md#kmiesniak)*
