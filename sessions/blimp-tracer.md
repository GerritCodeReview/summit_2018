# BLIMP Tracer: Integrating Build Impact Analysis with Code Review

__The Problem:__ Code review is a costly use of developer time. Developers minimize the cost by only carefully reviewing those patches that they deem worthy of effort and quickly skim the others. However, important decisions like these shouldn't be made only using gut feel.

__The Solution:__ We believe that patches that impact mission-critical deliverables or deliverables that span a broad set of products are riskier than others. To pinpoint such patches, we created BLIMP Tracer—a build impact analysis plugin that integrates tightly with code reviewing tools.

__Under the Hood:__  For any given patch, BLIMP Tracer traverses the Build Dependency Graph (BDG) to identify the deliverables that are impacted by the change. The identified set of deliverables are reported to developers within the code review interface.

__Evaluation:__ BLIMP Tracer is deployed by a product team at Dell EMC. To evaluate BLIMP Tracer, we surveyed and interviewed 45 developers, which reveals that BLIMP Tracer not only improves the speed and accuracy of identifying the set of deliverables that are impacted by a patch, but also helps the community to better understand the project architecture. 

*[Shane McIntosh, Assistant Professor / McGill University](../speakers.md#mcintosh)*
