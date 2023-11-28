# 7 Deployment view

??? info
    **Content**

    The deployment view describes:

    1. the technical infrastructure used to execute your system, with infrastructure elements like geographical locations, environments, computers, processors, channels and net topologies as well as other infrastructure elements and
    2. the mapping of (software) building blocks to that infrastructure elements.

    Often systems are executed in different environments, e.g. development environment, test environment, production environment. In such cases you should document all relevant environments.

    Especially document the deployment view when your software is executed as distributed system with more then one computer, processor, server or container or when you design and construct your own hardware processors and chips.

    From a software perspective it is sufficient to capture those elements of the infrastructure that are needed to show the deployment of your building blocks. Hardware architects can go beyond that and describe the infrastructure to any level of detail they need to capture.
    Motivation

    Software does not run without hardware. This underlying infrastructure can and will influence your system and/or some cross-cutting concepts. Therefore, you need to know the infrastructure.

    **Form**

    Maybe the highest level deployment diagram is already contained in section 3.2. as technical context with your own infrastructure as ONE black box. In this section you will zoom into this black box using additional deployment diagrams.

    * UML offers deployment diagrams to express that view. Use it, probably with nested diagrams, when your infrastructure is more complex.
    * When your (hardware) stakeholders prefer other kinds of diagrams rather than UML deployment diagram, let them use any kind that is able to show nodes and channels of the infrastructure.

    **Examples**

    * [Example Deployment View: Traffic Pursuit Unit](https://docs.arc42.org/examples/deployment-1/)
    * [Example Deployment View: HTML Sanity Checker](https://docs.arc42.org/examples/deployment-htmlsc-1/)
    * [Example Deployment View: Traffic Pursuit Unit Level 2](https://docs.arc42.org/examples/deployment-2/)

## 7.1 Infrastructure Level 1

??? info
    Describe (usually in a combination of diagrams, tables, and text):

    * the distribution of your system to multiple locations, environments, computers, processors, .. as well as the physical connections between them
    * important justification or motivation for this deployment structure
    * Quality and/or performance features of the infrastructure
    * the mapping of software artifacts (building blocks) to elements of the infrastructure

    For multiple environments or alternative deployments please copy that section of arc42 for all relevant environments.

    !!! abstract annotation "Infrastructure Level Template"

        !!! abstract annotation "Infrastructure overview diagram"
        !!! abstract annotation "Description of motivation or explanation in text form"
        !!! abstract annotation "(Optional) Description of quality or performance features"
        !!! abstract annotation "Description of mapping of building blocks"

!!! note "List of environment descriptions with template"

## 7.2 Infrastructure Level 2

??? info
    Here you can include the internal structure of (some) infrastructure elements from infrastructure level 1.

!!! note annotation "Please copy the structure from level 1 for each selected element"