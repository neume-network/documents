# social architecture of the neume network

- Type: Living document

## Purpose

This document outlines the neume network's architecture. It is created to

- increase the project's development velocity,
- increase quality and establish a vector of due diligence through upfront
  specification; and
- to ease onboarding for new neume contributors.

## Document Scope

The key words "MUST", "MUST NOT", "REQUIRED", "SHALL", "SHALL NOT", "SHOULD",
"SHOULD NOT", "RECOMMENDED", "MAY", and "OPTIONAL" in this document are to be
interpreted as described in RFC 2119.

The document's scope shall be limited to the neume network's architecture. A
descriptive style of writing is recommended.

## Context

The initial neume network architecture shall be created by building a socially
scalable indexing process for Ethereum-like networks with socially scalable,
herein, referring to the conscious design process of allowing many contributors
to work asynchronously and in parallel on the software project.

Whereas the neume network vision may potentially go beyond just indexing
Ethereum-like networks in that, e.g. its name suggests building an independent
"peer to peer network", for the initial version of this document, we want to
focus on establishing a solid foundation for a socially scalable and free (as
in libre) indexer first.

## Use of Programming Languages

With potential future exceptions, all neume network components shall be built
with the current latest version of the JavaScript programming language, and
specifically by making use of the node.js standard library.

The neume network shall be created through strict separation of concerns [1]
and with the Unix philosophy in mind [1, 2]:

```
- Write programs that do one thing and do it well.
- Write programs to work together.
- Write programs to handle text streams, because that is a universal interface.
```

Hence, meaningfully contributing to the node.js ecosystem means separating
logically connected components into modules and finally publishing those as
independent npm packages.

## Licensing

The neume network must use the GPL-3.0-only license wherever possible [3].
Whenever possible, contributors must be capable of retaining the copyright for
their submissions. Exceptions to the above statements must prioritize creating
interest-bearing effects for its contributors so as to ensure proper individual
incentivization for everyone helping to build the neume network.

## Contributing

Contributing to the neume network shall be doable and rewarding. The neume
network community acknowledges that intelligence is a social effect, despite it
feeling personal. We believe that solutions aren't invented so much as
discovered. Roadmaps and individual creativity are less important than a
reliable, shared process [6].

### Principles

#### Simplicity

A design must be simple, both in implementation and interface. It is more
important for the interface to be simple than the implementation [4].

#### Correctness

A design must be correct in all observable aspects. Incorrectness is simply
not allowed [4].

#### Consistency

The design must not be overly inconsistent. Consistency can be sacrificed for
simplicity in some cases [4].

#### Social Scalability

The design must be socially scalable. The design must be accessible, simple and
created with the limitations of human beings in mind such that it eases the
learning curve and potential risks for new contributors [5].

#### Agency over Upfront Consensus

All contributors shall ensure the highest degree of agency of fellow
contributors. Blockers like mandatory wait time or synchronous communication
shall be minimized. It is recommended to communicate via asynchronous and
descriptive mediums of communication (e.g. updating everyone via email vs.
doing a weekly all-hands call).

#### Testing for Confidence

All code shall be at least unit tested. All contributors must strive toward
improving the community's confidence in shipping new code to the main branch.

#### Automation over Chores

All contributors shall prioritize automation over chores. Implementations of
automation must be reproducible, sharable between contributors and (ideally)
tested.

### Safety

All neume network code repositories must include a `CODE_OF_CONDUCT.md`
document to allow contributing safely.

## References:

- 1: Dijkstra, Edsger W. "On the role of scientific thought." Selected writings
  on computing: a personal perspective. Springer, New York, NY, 1982. 60-66.
- 2: Raymond, Eric S. (2004). "Basics of the Unix Philosophy". The Art of Unix
  Programming. Addison-Wesley Professional (published 2003-09-23). ISBN
  0-13-142901-9. Retrieved 2016-11-01.
- 3: https://spdx.org/licenses/GPL-3.0-only.html
- 4: Worse is Worse, Jim Waldo, Sun Microsystems engineer
  https://www.artima.com/weblogs/viewpost.jsp?thread=24807
- 5:
  http://unenumerated.blogspot.com/2017/02/money-blockchains-and-social-scalability.html
- 6: Hintjens, Pieter. Social architecture: Building On-line Communities.
  CreateSpace, 2016. https://hintjens.gitbooks.io/social-architecture/content/
