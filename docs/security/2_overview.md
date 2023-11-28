# 2 Overview

??? info "Overview statement"
    Basically a summary of your project.

    Your overview statement is a very short explanation of what your project does. This should distinguish it from other potentially similar projects, and give an uninitiated stakeholder an easy path to understanding what they’re about to look at.

    Note that this isn’t intended to sell your project, it doesn’t need to be flashy and shouldn’t contain industry jargon. Write this with your least familiar audience in mind—most likely, your third-party auditors will know little about your particular niche.

    This statement is the first entry to the Overview section, and the rest will each get their own subheadings.

## 2.1 Background

??? info
    Context for why your project exists.

    We’ll use this section to provide information for reviewers who may not be familiar with your project's domain or problem area. This section can be more verbose, but try to keep it within reason! We want to communicate all of the key issues without giving the reader an excuse to skim over it.

## 2.2 Actors

??? info
    Different parts of your project that act upon each other.

    In this situation, Actors are not equivalent to Threat Actors. Instead of looking at the human element (actors using different parts of the system), this is looking at functional elements that are able to act upon each other.

    !!! quote "by TAG Security"
        These are the individual parts of your system that interact to provide the desired functionality. Actors only need to be separate if they are isolated in some way. For example, if a service has a database and a front-end API, but a vulnerability in either one would compromise the other, then the distinction between the database and front-end is not relevant.

        The means by which actors are isolated should also be described, as this is often what prevents an attacker from moving laterally after a compromise.

    Simply put: Write down any moving parts that are functionally independent.

## 2.3 Actions

??? info
    Details about how your actors act.

    After documenting the Actors, it’s time to show what their Actions are. This is a high-level description of how the actors interact with each other.

    If you have a more complex system, you may want to create a chart using a tool such as draw.io (the system used for the purpose of this demonstration has relatively low complexity, so the following example may be a bit overkill).

    If you find another way to communicate this for your situation, do what you think will best aid your readers in understanding the actions.

## 2.4 Goals

??? info
    What your project intends to do, and what security considerations are intended.

    While the Overview and Background sections help establish the core features of the project, the Goals section should describe what the project intends to accomplish. This includes both the end user value and the security goals for the project.

    Here’s an easy way to get started considering what your security goals might be. Think about areas where your software will do any of the following:

    1. Touch the internet
    2. Receive untrusted input
    3. Handle sensitive data

    In all likelihood, your list of goals will be much larger than the following example. Consider using a list or subheadings to segment points as needed (we provide an example in the Non-goals section, if you want to skip ahead to see that).

## 2.5 Non-goals

??? info
    What security considerations are not intended, and why.

    Non-goals are specifically security-related features that a user may consider to be within scope, but the project has intentionally marked it as out of scope for good reason. These may be responses to questions you’ve already been asked, but also try to anticipate any criticism and questions you might get from users or security auditors.

    Remember to keep these as detailed as possible, naming the concerns and then thoroughly addressing them.