# 5 Building Block View

??? info
    **Content**

    The building block view shows the static decomposition of the system into building blocks (modules, components, subsystems, classes, interfaces, packages, libraries, frameworks, layers, partitions, tiers, functions, macros, operations, data structures, …) as well as their dependencies (relationships, associations, …)

    This view is mandatory for every architecture documentation. In analogy to a house this is the floor plan.

    **Motivation**

    Maintain an overview of your source code by making its structure understandable through abstraction.

    This allows you to communicate with your stakeholder on an abstract level without disclosing implementation details.

    **Form**

    The building block view is a hierarchial collection of black boxes and white boxes (see figure below) and their descriptions.

    ![Scope and Context, Level 1 and Level 2 Diagram](https://docs.arc42.org/images/05-building-block-hierarchy.png)

    * Level 1 is the white box description of the overall system together with black box descriptions of all contained building blocks.
    * Level 2 zooms into some building blocks of level 1. Thus it contains the white box description of selected building blocks of level 1, together with black box descriptions of their internal building blocks.
    * Level 3 (not shown in the diagram above) zooms into details of selected building blocks of level 2, and so on.

    Examples

    * Example Building Block View: HTML Sanity Checker
    * Example Building Block View Level-1: Traffic Pursuit Unit
    * Example Building Block View Level-2: Traffic Pursuit Unit

## 5.1 Whitebox Overall System

!!! note annotation "Decomposition of system with white box template"

    Here you describe the decomposition of the overall system using the following white box template. It contains

    !!! abstract annotation "an overview diagram"
    !!! abstract annotation "a motivation for the decomposition"
    !!! abstract annotation "black box descriptions of the contained building blocks"
    
        For these we offer you alternatives:

        * use one table for a short and pragmatic overview of all contained building blocks and their interfaces
        * use a list of black box descriptions of the building blocks according to the black box template (see below). Depending on your choice of tool this list could be sub-chapters (in text files), sub-pages (in a Wiki) or nested elements (in a modelling tool).

        !!! info annotation "black box table"

            If you use tabular form you will only describe your black boxes with name and responsibility according to the following schema:

            | Name            | Responsibility |
            |-----------------|----------------|
            | __Black Box 1__ | __Text__       |
            | __Black Box 2__ | __Text__       |

        !!! info annotation "black box template"

            If you use a list of black box descriptions then you fill in a separate black box template for every important building block. Its headline is the name of the black box.

            Black Box Template:

            !!! abstract annotation "Purpose/Responsibility"

            !!! abstract annotation "Interface(s)"

            !!! abstract annotation "(Optional) Quality/Performance Characteristics"

            !!! abstract annotation "(Optional) Directory/File Location"

            !!! abstract annotation "(Optional) Fulfilled Requirements"

            !!! abstract annotation "(Optional) Open Issues/Problems/Risks"


    !!! abstract annotation "(optional:) important interfaces, that are not explained in the black box templates of a building block, but are very important for understanding the white box."

        Since there are so many ways to specify interfaces why do not provide a specific template for them.

        In the best case you will get away with examples or simple signatures.

## 5.2 Level 2

??? info
    Here you can specify the inner structure of (some) building blocks from level 1 as white boxes.

    You have to decide which building blocks of your system are important enough to justify such a detailed description. Please prefer relevance over completeness. Specify important, surprising, risky, complex or volatile building blocks. Leave out normal, simple, boring or standardized parts of your system

!!! note annotation "List of white box descriptions for each building block"

    Specifies the internal structure of a building block of level 1.

    Use the white box template (see above).

## 5.3 Level 3

??? info
    Here you can specify the inner structure of (some) building blocks from level 2 as white boxes.

    When you need more detailed levels of your architecture please copy this part of arc42 for additional levels.

!!! note annotation "List of white box descriptions for each building block of level 2"

    Specifies the internal structure of a building block of level 2.

    Use the white box template (see above).