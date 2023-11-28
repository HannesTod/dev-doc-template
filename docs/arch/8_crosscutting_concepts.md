# 8 Crosscutting Concepts

??? info
    **Content**

    This section describes overall, principal regulations and solution ideas that are relevant in multiple parts (→ cross-cutting) of your system. Such concepts are often related to multiple building blocks. They include many different topics, such as

    * domain models
    * architectural patterns or design patterns
    * rules for using specific technology
    * principale, often technical decisions of overall decisions
    * implementation rules

    **Motivation**

    Concepts form the basis for conceptual integrity (consistency, homogeneity) of the architecture. Thus, they are an important contribution to achieve inner qualities of your system.

    Some of these concepts cannot be assigned to individual building blocks (e.g. security or safety). This is the place in the template that we provided for a cohesive specification of such concepts.

    **Form**

    The form can be varied:

    * concept papers with any kind of structure
    * cross-cutting model excerpts or scenarios using notations of the architecture views
    * example implementations,especially for technical concepts
    * reference to typical usage of standard frameworks (e.g. using Hibernate for object/relational mapping)

    **Structure of this Section**

    A potential (but not mandatory) structure for this section could be:

    * Domain concepts
    * User Experience concepts (UX)
    * Safety and security concepts
    * Architecture and design patterns
    * “Under-the-hood” concepts
    * Development concepts
    * Operational concepts

    !!! annotation note "It might be difficult to assign individual concepts to one specific topic on this list."

    ![Crosscutting concepts diagram](https://docs.arc42.org/images/08-Crosscutting-Concepts-Structure.png)

    **Background**

    Some topics within systems often concern multiple building blocks, components or elements. It might be easier to communicate or document such cross-cutting topics at a central location, instead of repeating them in the description of the concerned elements.

    Certain concepts might concern all elements of a system, others might only be relevant for a few. In the diagram below, logging concerns all three components, whereas security is relevant only for two components.

    ![Crosscutting concerns diagram](https://docs.arc42.org/images/concepts/crosscutting_concerns.drawio.png)

    Some real-life examples:

    * Within a system, a common format for log-messages shall be established, combined with a common convention of choosing the appropriate log-destination. These decisions, along with implementation examples, could be described as “logging-concept”.
    * A system has numerous backend services, that communicate among each other based upon remote procedure calls or http-based REST. Calling services (“consumers”) always need to authenticate themselves to the called service (“provider”). For this authentication, a central common authorization service has to be used. The technical and organizational details such authentication could be described as “backend authentication concept”.
    * (taken from the HTML Sanity Checker, see below): All (7+) checker components within the system are structured according to the strategy pattern.

    **Examples**

    * [Example Concept: HTML Sanity Checker (Domain + URIs)](https://docs.arc42.org/examples/concept-htmlsc-1/)
    * [Example Concept: HTML Sanity Checker (Multiple Checking Algorithms)](https://docs.arc42.org/examples/concept-htmlsc-2/)
    * [Example Concept: TrafficPursuitUnit Domain Entity Model](https://docs.arc42.org/examples/concept-tpu-1/)
    * [Example Concept: TrafficPursuitUnit, Event Handling](https://docs.arc42.org/examples/concept-tpu-2/)

!!! note annotation "Description of concepts"