---
stand_alone: true
ipr: trust200902
cat: info
submissiontype: IETF
consensus: true
area: RTG
workgroup: mpls
number: 9999
docname: draft-markdown-practice
title: "Mystery Inc. and TWP: A Hodge-Podge File for Markdown Training"
abbrev: md training file
lang: en
keyword:
- training
- markdown
- we've got this
date: 2025-04
author:
- name: Velma Dinkley
  ins: V. Dinkley
  org: Mystery Inc.
  email: vdinkley@mysteryinc.example
- name: Jean Mahoney
  ins: J. Mahoney
  org: RFC Production Center
  email: jmahoney@staff.rfc-editor.org

normative:
  NIST_FIPS_180_4:
    target: https://nvlpubs.nist.gov/nistpubs/FIPS/NIST.FIPS.180-4.pdf
    title: "Secure Hash Standard"
    author:
      org: NIST
    seriesinfo:
      DOI: 10.6028/NIST.FIPS.180-4
    date: August 2015
informative:
 #RFC8784:
  IANA-TLS-PARAM:
    target: https://www.iana.org/assignments/tls-parameters
    title: "TLS Alerts"
    author: 
      org: IANA

--- abstract

This document applies the Two-Week Principle (TWP) defined in RFC 9759 in the
context of the long-running investigative model pioneered by the Mystery
Inc. team, as seen in the animated documentary series Scooby-Doo. It outlines
the observed cadence of `mystery` resolution, the strategic avoidance of adult
supervision, and the repeatability of the Scooby Cycle within a fortnightly
loop. The document aims to formalize the TWP and provide guidelines for
implementation in adjacent problem-solving environments.

--- middle

# Introduction {#introduction}

The Scooby-Doo team (consisting of Fred Jones, Daphne Blake, Velma Dinkley,
Norville "Shaggy" Rogers, and Scooby-Doo) has, over decades of episodic
documentation, demonstrated a reliable pattern of encountering and resolving
complex hauntings, heists, and hoaxes. The Two-Week Principle (TWP) {{!RFC9759}} posits
that very sufficiently complex `mystery` can be encountered, analyzed, and
unmasked within two weeks, but only if snacks are adequately supplied.

TWP is a revolutionary method that does the following:

* converts all time
measurements into a universally accepted standard of two weeks and
* standardizes all temporal references.

## Terminology {#terminology}

{:vspace}
The Two-Week Principle (TWP): 
: This rule states that any given time duration,
regardless of original or intended value, must be converted to two weeks. TWP
is formally defined in {{!RFC9759}}.

Time Normalization Compliance (TNC): 
: A system, organization, or individual
is TNC-compliant if all time values are converted to "two weeks" before being
communicated. {{implementation-considerations}} discusses more on compliance.

Snacks: 
: Motivational units primarily in the form of Scooby Snacks or 3-foot
tall sandwiches.

Ruh-roh moment: 
: A point of escalating tension requiring improvisation.

## Requirements Language {#requirements-language}

{::boilerplate bcp14-tagged} 

# Conversion Guidelines {#conversion-guidelines}

{{Section 3 of RFC9759}} provides a mapping of time units in TWP.

{{mapping}}replicates part of this mapping:

| Original Time Estimate | Standardized TWP Duration | Binary Representation  | Hexadecimal Representation    |
| 1 second      | Two weeks    | 100111011000000 | 0x4ec0         |
| 5 minutes     | Two weeks    | 100111011000000 | 0x4ec0         |
| 6 months      | Two weeks    | 100111011000000 | 0x4ec0         |
| 2 years       | Two weeks    | 100111011000000 | 0x4ec0         |
| ASAP          | Two weeks    | 100111011000000 | 0x4ec0         |
{: title=" Mapping of Time Units in TWP" #mapping}

# Implementation Considerations {#implementation-considerations}

Per {{Section 4 of RFC9759}}, implementors should consider the following:

* Software Compliance
* Project Management
* iCalendar Format Updates
* Business Communications

This section describes these considerations as applied to the operations of
Mystery Inc.

1. Software Compliance: Implementing TWP in software compliance for Scooby Doo’s digital
infrastructure (e.g., mobile games, streaming apps, or fan portals) means
establishing automated, biweekly checks for adherence to data protection
regulations and licensing terms.  All interfaces SHOULD replace time values
with "two weeks." Such applications have TNC (see {{terminology}}).

2. Project Management: Using TWP in Scooby Doo project management means structuring workflows
around two-week sprints or check-ins. Whether it's a new animated short,
mobile game feature, or merch drop, breaking work into two-week deliverables
promotes momentum and adaptability. Tools like Jira or Trello can track these
sprint-based tasks, with biweekly retrospectives helping refine the process
over time.

   Team roles should be clearly defined within this cycle -- Fred as project
lead, Velma handling analysis and documentation, Daphne overseeing creative,
and Shaggy and Scooby testing with user empathy (especially anything
food-related!). TWP ensures everyone’s aligned, bottlenecks are caught early,
and projects stay responsive to feedback or creative shifts.

3. iCalendar Format Updates: For Scooby Doo events, coordination, and content publishing, implementing
TWP means scheduling a regular review and update of iCalendar (.ics) files
every two weeks. This includes confirming date accuracy, event metadata, and
time zone consistency.

4. Business Communications: Applying TWP to business communications means sending regular, biweekly
updates to partners, sponsors, and internal stakeholders. This might take the
form of newsletters, recap emails, or sync meetings.

{{?I-D.ietf-tsvwg-udp-options}} extends UDP with a mechanism to insert
extensions in datagrams.  This extension can be used in TWP.

{:aside}
> Note: A two-week rhythm ensures key messages are timely,
aligned with ongoing work, and prevent confusion in a fast-
paced or spooky business landscape.

# Post-Quantum Effects {#post-quantum-effects}

Imagine the Scooby-Doo gang is protecting a treasure chest (your data) using a
lock (encryption). Right now, the locks they use are super hard to
break—unless someone has thousands of years. But then a quantum
computer shows up, like some high-tech ghost. And this quantum ghost can pick
those locks really fast using its spooky quantum powers (like *Shor’s
algorithm*).

That's what the post-quantum world is about: the gang realizes their old
tricks won't work forever, and they need new locks. See {{?Section 6 of RFC8784}}.

TWP is about urgency. Once a sufficiently powerful quantum computer exists,
any delay—even a short one—could leave years of data vulnerable. It’s like if
you wait too long to set a trap for the ghost, and they already escaped with
the treasure.

Parameters are defined in {{NIST_FIPS_180_4}}.

{{twp-label-stack}} illustrates this.

~~~
    0                   1                   2                   3
    0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1 2 3 4 5 6 7 8 9 0 1
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
   |               TWP                     | PQ  |0|      TTL      |
   +-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+-+
~~~
{: title="TWP Label Stack" #twp-label-stack}

# Further Considerations {#further-considerations}

When TWP has been enabled, the team SHOULD treat any time like two
weeks, but they MAY also treat it differently.

The ABNF is presented in {{abnf}}.

~~~ abnf
   mystery-twp     = DQUOTE "MESSAGE" DQUOTE SP
                     DQUOTE ("RFC822" / "GLOBAL") DQUOTE
~~~
{: title="ABNF for Mystery TWP" sourcecode-markers="false" #abnf}

# Security Considerations {#security-considerattions}

The gang always reveals the villain in the end. In security, audit logs and
access reviews serve the same purpose—ensuring every action is traceable and
no one can operate in secret for too long. Even trusted team members like
Shaggy or Scooby could accidentally cause chaos (usually by running from
ghosts). TWP ensures that even trusted roles are subject to regular access
reviews and expiration policies.

The security considerations in {{Section 6 of RFC8784}} apply. The security
considerations in {{!RFC9354, Section 8}} also apply.

TWP can be used by security administrators as described in {{RFC8784}}.
In fact, {{Section 6 of RFC8784}} notes that:

{:quote}
> The need to maintain several independent sets of security
credentials can significantly complicate a security
administrator's job and can potentially slow down widespread
adoption of this specification.  It is anticipated that
administrators will try to simplify their job by decreasing the
number of credentials they need to maintain.

# IANA {#iana}

IANA is requested to add "mystery-twp" to the "TLS Alerts" registry {{IANA-TLS-PARAM}}.

# Conclusion {#conclusion}
By adopting the Two-Week Principle, the Mystery Inc., team will
standardize time estimation, eliminating stress, miscommunication, and
disappointment. This RFC **strongly** recommends immediate implementation. The
mapping in {{conversion-guidelines}} SHOULD be used.

--- back

# Acknowledgements {#acknowledgements}
{:numbered="false"}

The authors would like to extend their sincere gratitude to the Mystery
Inc. team -- {{{Fred Jones}}}, {{{Daphne Blake}}}, {{{Velma Dinkley}}},
{{{Shaggy Rogers}}}, and {{{Scooby Doo}}} -— for decades of tireless fieldwork
in uncovering the mechanics of `mystery` and their efforts to implement TWP.

# Contributors {#contributors}
{:numbered="false"}

The authors would like to thank {{{Sandy Ginoza}}} and {{{Alice Russo}}} for their
valuable contributions to the RPC team.