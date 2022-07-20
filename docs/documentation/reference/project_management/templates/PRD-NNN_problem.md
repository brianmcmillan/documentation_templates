---
title: PRD-### { Title }
---
<!---
The Problem Reference Document (PRD) is used to record the high level problem and associated requirements for a potential project. This document will be used to help facilitate prioritization decisions. NOTE: This document is only one potential method for documenting this information and the team will need to figure out what process and documents work best in their particular situation.

File name: PRD-###_<TITLE>.md
--->

!!! tldr "TL;DR"  
    { Lorem ipsum dolor sit amet }  

    **IN ORDER TO** { ... }  
    **AS A** { ... }  
    **I WANT** { ... }  

!!! info  
    **Status:** { **CREATED** | IN REVIEW | STARTED | COMPLETED | CANCELED }  
    **Business Contact Name:** { name }  
    **Business Contact email:** { email }  
    **Technical Contact Name:** { name }  
    **Technical Contact email:** { email }  
    **Other contributors:** { email }  
    **Linked RFC:** [RFC-###]()  

| Created Date | Reviewed Date |  Canceled Date | Started Date | Completed Date |
|---|---|---|---|---|
|{ YYYY-MM-DD }|{ YYYY-MM-DD }|{ YYYY-MM-DD }|{ YYYY-MM-DD }|{ YYYY-MM-DD }|

### Prioritization Scoring
<!--- At this point in the project life cycle, we are estimating the rough costs associated with this feature for prioritization purposes only. The scoring values are always in the context of other opportunities and should be rescored on each evaluation.  --->

<!---One scoring method is to use a modified Fibonacci sequence for each value (1, 2, 3, 5, 8, 13, 21). Benefits and Urgency are scored highest to lowest (lowest benefit = 1) and Duration is scored lowest to highest (e.g. shortest duration = 1). See Ch. 9: Final Iteration - Innovation and Planning in the book "Building Data Products: Introduction to Data and Analytics Engineering for non-programmers"  --->
|Benefit Value (B) | Urgency Value (U) | Duration Value (D) | Score (B*U)/D) |
|---|---|---|---|
|{ # }|{ # }|{ # }|{ # }|

<!---An alternative scoring method: The value assigned to the project is determined by providing each stakeholder an equal amount of money to spend on any of the features being evaluated with this process. The total amount in the pool is determined by multiplying the number of developers times the number of months in the timeframe (e.g. 10 developers * 3 months * $5 = $150 total). If you have five people making the prioritization decisions, then the $150 is divided by five. This provides each person $30 to vote with.

**Resource estimate:** { XX people }  
**Time estimate:**  { XX time }  
**Feature cost:** { $5 per FTE per month * time * people }  

### Final business value score: { $## }  
--->

### Background
<!--- The background section provides the reader with helpful context before diving into the problem domain. Provide sufficient details to properly educate the reader on the problem domain. In order for a reader to understand the content of the PRD, they must first understand the context. That context setting is the goal of the background section. Visual explanations are encouraged if applicable.--->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

### Problem Statement
<!--- This is the heart of the PRD as it simplifies the user research into clear problem statements. Each of the problems should clearly map to the problems identified by the user research and the corresponding personas defined below. The personas should be generalized versions of the actual interviewed users.

What is the measurable business benefit of solving this problem considering the stated scope and appetite? Ideally, this would be expressed in financial value. Typically expressed as changes in  revenue, raw material cost, investment / inventory, or operational expenses. Additionally, consider the timeframe over which this benefit will be realized.--->

**We would be dumb if we didn't** {  Lorem ipsum dolor sit amet }  
**Because it** {  Lorem ipsum dolor sit amet }  
**And affects** {  Lorem ipsum dolor sit amet }  
**Resulting in** {  Lorem ipsum dolor sit amet }  
**A successful solution would** {  Lorem ipsum dolor sit amet }  
**Within** { time frame }  
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

### Stakeholders
<!--- This section is the most important as it grounds the PRD in real, experienced user problems. For the author the goal of this section is to collect high-quality research which will be used to identify common patterns across users. The better the research, the easier it is to determine patterns, and the simpler the problem statement can be. For readers this section sets a concrete context for understanding the core problem.--->

#### User Research
<!--- Describe the user research methodology. --->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

#### Personas
<!--- At a bare minimum, each persona should articulate the problem or job being done. --->
* Persona 1 has troubles { doing what } with this problem.  
* Persona 2 has troubles { doing what } with this problem.  
* Persona 3 has troubles { doing what } with this problem.  

### Requirements
<!--- These are the high level outcome focused stories describing the business context, personas, and acceptance criteria for the problem. --->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

!!! summary "Story 1 - Title"
    **IN ORDER TO** { ... }  
    **AS A** { ... }  
    **I WANT** { ... }  
    **GIVEN** { ... }  
    **WHEN** { ... }  
    **THEN** { ... }  
    **Considerations:** { Lorem ipsum dolor sit amet }  

!!! summary "Story 2 - Title"
    **IN ORDER TO** { ... }  
    **AS A** { ... }  
    **I WANT** { ... }  
    **GIVEN** { ... }  
    **WHEN** { ... }  
    **THEN** { ... }  
    **Considerations:** { Lorem ipsum dolor sit amet }  

#### Business Appetite
<!--- How much time do we believe we should spend addressing this problem? This lets the business owners convey how much investment they feel is worth risking.--->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

#### Technical Duration
<!--- How much time does the technical team believe would be required to achieve the business benefit? Consider the Appetite, risk, and complexity. This isn't used as a commitment but as part of the prioritization process. --->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

----

### Solution
<!--- Brief description of the solution. Be careful to not be overly specific.--->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

#### Breadboard architecture
<!--- *Rough* drawings of the solution UX and / or architecture, sufficient to convey the initial design.--->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

````mermaid
flowchart TB
    PERSON---ORDER
    ORDER---LINE_ITEM
    PERSON-.-DELIVERY_ADDRESS
    ORDER---SHIPPING---DELIVERY_ADDRESS
````

#### Fat Marker mock-ups
<!--- *Rough* drawings of the solution UI, sufficient to convey the initial design.--->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  
![Image 1]()  
![Image 2]()  

#### Rabbit holes
<!--- Are there any risky aspects to this problem or solution you can call out early in the process? how should they be addressed?--->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

#### No Gos
<!--- Identify the things you are *not* including as part of the solution.--->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

----

### References and notes
<!--- Is there any additional information that would be useful? --->
{ Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor. }  

----
[HashiCorp's Problem Requirements Document](https://works.hashicorp.com/articles/prd-template)  
[Basecamp - Shape Up](https://basecamp.com/shapeup)  