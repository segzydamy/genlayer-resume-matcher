# GenLayer Intelligent Candidate Screening & Resume Matcher

An on-chain Intelligent Contract deployed on GenLayer Testnet that leverages decentralized LLM consensus to evaluate job applicant credentials, experience, and domain skills against technical role requirements.

## Overview
Recruiting in decentralized ecosystems faces high volumes of unverified applications. This contract automates fair, unbiased, and objective applicant screening using GenLayer's Optimistic Democracy.

## Features
- **Decentralized AI Screening:** Employs `gl.nondet.exec_prompt` and `gl.eq_principle.strict_eq` across validator nodes.
- **Match Scoring:** Computes an objective fit score and issues clear `SHORTLIST` or `REJECT` verdicts.
- **Native GenVM Storage:** Stores immutable applicant evaluations using `TreeMap` and `u32` primitives.

## Functions
- `submit_application(candidate_name, target_role, skills_summary, experience_years)`: Write method submitting applicant profile for AI consensus scoring.
- `get_candidate_evaluation(app_id)`: View method returning candidate evaluation details and scores.
- `get_recruiting_stats()`: View method returning aggregate application and shortlisting statistics.

## Deployment Details
- **Network:** GenLayer Testnet
- **Contract Address:** `0x324abA5151AE4E6941aa5d1DB6fF2f831D6621F7`
- **Explorer:** [View on GenLayer Studio Explorer](https://explorer-studio.genlayer.com/address/0x324abA5151AE4E6941aa5d1DB6fF2f831D6621F7)
- **Runtime:** Python (GenVM)
- **Status:** Finalized
