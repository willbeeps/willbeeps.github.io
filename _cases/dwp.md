---
layout: case
title: "DWP"
sector:       "Government"
organisation: "Department for Work and Pensions"
role: "Lead UX Consultant / Service Designer"
brief: "Discovery and private beta to reduce friction for applicants and caseworkers handling a key working-age benefit claim."
kicker: "A discovery and private beta to reduce friction for applicants and caseworkers handling a key working-age benefit claim — automating eligibility decisions on a legacy payment system without touching the legacy payment system."
tags:
  - DWP
  - Service design
  - Discovery & private beta
status: "Shipped"
status_note: "Private beta, internal"
date_range: "2022–2023"
date_note: "15-month engagement"
outcomes:
  - key: "Case throughput"
    value: "+38%"
    note: "Measured against the pre-pilot baseline over eight weeks."
  - key: "Caseworker touchtime"
    value: "−6m 12s"
    note: "Median time from claim received to decision issued."
  - key: "Applicant drop-off"
    value: "−14pts"
    note: "On the ID verification step — the deepest trough in the funnel."
position:
  - User research
  - Service design
image: /assets/images/dwp.png
image_alt: DWP logo
date: 2022-01-10
protected: true
featured: false
---

## Automation for NSJSA: private beta & discovery ##

### Outcome ###
Designed a service to remove points of friction and effort for both applicants and civil servants, with automated ID verification and eligibility decisions.
Our research showed that even a limited public beta was dependent on a shared ID verification service (within DWP) that wasn’t meeting user needs, and I created a set of requirements for the shared service team  
The design of the service - showcasing, essentially, how its limitations were due to the underlying architecture - highlighted to the Deputy Director the urgency of the need to invest in backend technology, so we won the opportunity to deliver a further discovery around full automation. 

### Challenge ###
Benefits processing is dependent on JSAPS - the Jobseekers Allowance Payment System - a system from the 90s (and possibly older than that), which DWP re-platformed a few years ago. 

I arrived on the project at the start of a private beta, when the team was building on an alpha to automate the eligibility decision for jobseekers allowance, one of the benefits processed through JSAPS. This private beta would deliver: 
- automation of non-entitled claims
- automated new claim caseload management
- Automated fraud check
The service, as you might expect, had a lot of complexity to resolve, a lot of which revolved around integrating with their ML/robotics decisioning, and implementing fraud reduction policy, along with how this is communicated to citizens. 

### Actions ###
I worked within a cross-functional team - BAs, content designer, SMEs, tech architect, interaction designer, and a Product Manager

    {% include figure-showcase.html
       label="FIG. 01 - Service blueprint"
       title="The system map that unlocked the conversation"
       description="Drawn across three workshops, this became the shared reference point for every decision about automation scope."
       image="/assets/images/dwp_blue.png"
       alt="NSJSA service flow diagram, V4, November 2024"
    %}

The work covered a number of scenarios related to the application - e.g. duplicate applications, data mismatches, and a 3-sprint spike into online ID verification, where I was tasked with scoping, planning, conducting, synthesising and advocating for any changes required, which involved engaging many teams around the department.

### Learnings ###
JSAPS is very expensive to maintain, and although Automation would resolve some of the issues with JSAPS, it still required a human agent to interact with it, which would mean a good chunk of the most time-consuming aspects of the role would continue, and JSAPS would need to remain as the critical part of system architecture.

![A gap analysis of the service](/assets/images/dwp_gaps.png)

Additionally, the research found that although we were able to resolve issues related to communicating application progress, the requirement to use a shared ID verification service, which could not be introduced into the application journey in a way that would avoid asking duplicative questions to users, created a lot of friction that could risk increasing drop-out rates. 

![A sprint-by-sprint review of findings and decisionst](/assets/images/dwp_review.png)

These issues were presented in our end-of-private-beta playback, after which we were commissioned to run a further mini-discovery  to see whether anything had changed in the process or policy related to how claims were assessed, so that we could start an alpha that looked to bypass JSAPS altogether. 

