# TeamDzmitry  - We need a team name change.

**OReilly Architecture Kata Spring 2022**

Ed's notes

## Analogy
Infrastructure provider and operations aggregator

Example:
1. County fairgrounds
   1. Provides infrastructure - customer parking, electricity, bathrooms, security
   2. Vendors = our Non-profits
   3. Customers = their clients / trainees

## [Candidate](Candidate.md)
This is supposed to be for bringing 'diversity' into lucrative tech jobs.  I read that as Black and Hispanic underrepresented groups.
As an exercise, I am also thinking of other disadvantaged groups like homeless, veterans, alcoholics, women living in shelters.

Since some groups might have special need protections like AIDS status, criminal backgrounds, etc. there is a need to protect personal info.
### Candidate injestion
Pipeline -- 'pull'
1) high schools
2) VA - Veterans Administration
3) churches
4) jails

## [Nonprofits](NonProfits.md)

## [Services](Services.md)

## Forces
1) Need to protect candidate personal info
2) Learnability - non-profit operators tend to not have tech skills.  Different skill sets.
3) Compatibility - integrating lots of different external systems - health (e.g. hospitals, clinics), law (jails and police), education (schools and universities)
4) Simplicity - easy to add candidates and nonprofits.  easy to remove.
   1) Non-profit - some guy starts a non-profit, added to our infrastructure, after 3 months decides that it's not for him.  Closes the non-profit.  Must remove it.
   2) Some candidates might be in marginal situations (e.g. in/out of rehab, homeless - on the move) and have to start and stop suddenly
   

# Architecture suggestions

The need to segregate candidate data with rapid and easy inclusion suggest that persisted data be kept segregated.

** Separate data store / Databases **

Because money will be involved, much stricter security or integration with secure financial services is required.

1) Micro-services
   1) separate databases
2) Microkernel
   1) rapid plug-in = non-profits