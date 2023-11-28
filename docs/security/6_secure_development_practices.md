# 6 Secure Development Practices

??? info "Summary statement"
    This section has three values. After providing the summary statement, we’ll nest the other two values beneath subheadings, with narrative explanations for each section.

    Secure development practices overview

    * Development pipeline (SDLC, provenance, etc.)
    * Communication channels (community, collaboration, etc.)

## 6.1 Development Pipeline

??? info
    What security practices do you automate or enforce in your SDLC?

    Here are some things you might consider including:

    * Do you have branch protection or repo security features in place?
    * Are committers required to sign their commits, or a contributor license agreement?
    * Do you have automated testing or fuzzing on every pull request?
    * Do you have software composition analysis or dependency management tooling?
    * How many reviewers are required for a pull request to be approved?
    * Do you have any measures around code owners?
    * Is your release process automated?
    * Does every release include an automatically generated Software Bill of Materials?
    * Do you sign releases?
    * Are container images immutable and signed?

## 6.2 Communication Channels

??? info
    This section should paint a picture of how the project communicates. Use the following sections to document things like Slack channels, recurring meetings, mailing lists, and so forth.

    * Internal  
      How do team members communicate with each other?
    * Inbound  
      How do users or prospective users communicate with the team?
    * Outbound  
      How do you communicate with your users?