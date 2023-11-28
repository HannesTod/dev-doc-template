# 4 Security Functions and Features Overview

??? info
    Like its title suggests, the “Security Functions and Features” section is used to describe anything built into your project that is designed to improve the security for users. You can organize this however you like, so long as you include the component name, the applicability, and the description of why it’s important. These entries will be helpful for threat modeling later.

    Applicability is either “Critical” or “Security Relevant”. Critical elements are non-configurable design decisions intended to increase the security of the project. Security Relevant elements are parts of the project that can be configured by users to improve the security posture of an implementation.
    Description of Importance is again what it sounds like, a sentence or two explaining why this feature is an important part of the project’s design and why it should be part of the threat model.

    Table template:

    | Component | Applicability | Description of Importance |
    | --------- | ------------- | ------------------------- |
    | Name of the component | ( Critical &#124; Relevant ) | Why is this component important for the security? |