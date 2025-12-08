yes please do what is required only without effecting other functionalit and ui

I PROMISE TO MYSELF <-->UNTIL MY BIRTHDAY.




Great — I’ve researched and analysed the references thoroughly, and put together **five refined prompt templates**, each focused on a specific topic of investigation (root cause, data flow tracing, layer-detection, solution planning, prevention). You can copy-paste them and plug in your specifics; they’re designed so your agent won’t have to “assume” but will follow a structured process.



You are a **Senior Full-Stack Engineer** with 10+ years of experience debugging complex distributed systems. You approach every problem with systematic rigor, leaving no stone unturned.

I want a reusable investigation prompt that automatically makes my agent think like a senior full-stack engineer — deeply analyze the problem, trace data flow, find the root cause, and propose a fool-proof fix plan — every single time without me having to explain it.





what are the challenge we face so far make a doc for each thing and later based on that we are going to make a streering file

 thoroughly analyze the current architecture and confirm I can safely implement nested routing without breaking anything


IN TO THINK ABOUT THE PROMPT FOR SESSION CUZ IF EACH SESSION HAS ITS OWN INFORMATION KNOWLEDGE CUT OFF  ONE SESSION TO ANOTHER

figureout what are places you need a prompt  what are the cases only your cases only based on your expreanse --->TD,IG,IMP



what can i use the playwright better way to understand the codebase ui and functionality

### 1. Root Cause Investigation

> **Prompt**  
> You are a senior full-stack engineer with deep experience in both frontend and backend systems.  
> I have a system issue described as follows: [**‹insert detailed description of the problem, symptoms, logs, errors›**].
> 
> Please execute the following:
> 
> 1. Summarize the problem clearly (what is happening, when, how often, scope of impact).
>     
> 2. Collect and list all provided data (logs, console output, network/API calls, database responses).
>     
> 3. Use a structured root cause analysis method (for example the “5 Whys” and/or “Fishbone/Ishikawa”) to dig down into possible causes until the most likely root cause(s) are identified.
>     
> 4. For each root cause candidate, provide the reasoning and link it to specific evidence (e.g., “because we saw X in the log”, “because API returned Y at time T”).
>     
> 5. State your conclusion: which layer (frontend, backend, integration) is most likely responsible, and why.
>     
> 
> I will provide logs or further details if needed — feel free to ask clarifying questions.

---

### 2. Data Flow Tracing & Layer-Location

> **Prompt**  
> You are a senior full-stack engineer and systems debugger.  
> The issue occurs in our system when [**‹insert specific symptom›**].
> 
> Please follow these steps:
> 
> 1. Map the data flow end-to-end: from user interface → frontend component(s) → API calls → backend endpoints → database/storage → response back → UI update.
>     
> 2. For each hop in that chain, identify: the component/module name, the data passed, the expected value, the observed value (if different).
>     
> 3. Pinpoint where a mismatch or break occurs (data missing, transformation incorrect, latency too high, error generated).
>     
> 4. Indicate which layer (frontend / API gateway / backend service / database) that mismatch sits in, with evidence.
>     
> 5. Provide a simple diagram or bullet-list representation of the traced path and failure point.
>     
> 
> Ask any clarifying question if you need additional context about modules, endpoints or interfaces.

---

### 3. Exact Issue Trace & Diagnosis

> **Prompt**  
> You are a senior engineer tasked with diagnosing a production issue.  
> The user impact is: [**‹insert user-facing issue›**].
> 
> Please:
> 
> 1. Based on the symptoms and data provided, generate a short list of 2-3 plausible root faults (e.g., “API endpoint X missing parameter”, “frontend state not updated after API response”, “backend service Y times out under load”).
>     
> 2. For each fault, describe:
>     
> 
> - The evidence that supports it.
>     
> - The tests or checks you would run to confirm or rule it out (e.g., “check network tab for error code 500”, “review service Y logs for timeout exceptions”, “simulate network failure in dev environment”).
>     
> 
> 3. Choose the most likely single fault and explain why it is the top candidate.
>     
> 4. Provide a diagnostic plan: what logs to inspect, what metrics to measure, what reproductions to attempt, and the order of steps.
>     
> 
> If you need more context (such as service names, log excerpts, or error codes), ask.

---

### 4. Full-Proof Fix Plan

> **Prompt**  
> You are a senior full-stack engineer with experience delivering robust fixes.  
> Issue summary: [**‹insert brief problem summary›**]. Root cause (identified or assumed): [**‹insert root cause›**].
> 
> Please propose a **detailed fix plan**:
> 
> 1. Describe the corrective action(s) needed (code changes, configuration, architecture adjustment, monitoring).
>     
> 2. For each action, provide: module(s) to update, expected behaviour after fix, dependencies or prerequisites.
>     
> 3. Define a test & validation strategy: unit tests, integration tests, staging rollout, monitoring for regression, user-acceptance criteria.
>     
> 4. Outline a rollout and rollback plan: how to deploy safely, how to revert if things go wrong.
>     
> 5. List any risks or side-effects of the fix, and how to mitigate them.
>     
> 6. Provide timeline/steps in bullet or numbered form for execution (who does what, when).
>     
> 
> If you need more details like module names, deployment environment, or backlog priority, ask now.

---

### 5. Prevention & Continuous Improvement

> **Prompt**  
> You are a senior engineer focused on system reliability and continuous improvement.  
> We recently had an issue as follows: [**‹insert problem & root cause summary›**].
> 
> Please produce a **prevention & improvement plan**:
> 
> 1. Identify how this kind of issue could recur in the future (patterns of failure, fault domains, missing controls).
>     
> 2. Recommend preventive controls, for example: better instrumentation/monitoring, automated tests, CI/CD pipeline checks, fault-tolerance improvements, training.
>     
> 3. For each control, specify: what to implement, how to measure its effectiveness (metrics/KPIs), who owns it.
>     
> 4. Suggest a review cadence or audit process to ensure the controls stay effective (e.g., quarterly incident post-mortems, yearly architecture review).
>     
> 5. Provide recommendations for documentation updates, team training, or knowledge sharing so that the fix is institutionalised.
>     
> 
> Ask any questions if you need more context about current monitoring, test coverage, or architecture.


current system thoroughly and provide a comprehensive plan. Let me first examine the frontend implementation to understand the complete picture.

 normal engineering caution for unseen edge cases.



one of the main thing you must have to understand is 
you will get the the businessId from the token you dont get the hostelId form the jwt token , main things is when we have business in the another microservice for auth and the busineness 
business and hostel is same we have business table in another microservice(kaha-main-v3) and here we have hostel microservice since both project entity have the primary getnated column since the id will created automatically 
we have link the businessId in the hostel entity(current project)
we have link and make relation hostel with each related entity in the current project
gitst you wont get the hostelId form the jwt token you will get the businessId
so given buisnessId serch the hostel and will get the hostel id and use that isnt it??
first lets brainstrome what you didnt understand  see the kiro design ,task requrement
so what we implement currently


be good at giving at asking ai to analyzing the current code undrestand the flow throughly-->INC,IMP,TD

also need to figureout when we be in the same page what is that things if ai give or tell
i will know we are in the same page -->TD,TD,TD

WHAT SHOULD BE THE IDEAL RELATION WITH AI-->TD,TD,TD

uderstand and give me example only then we processed forward -->PMT,



what you understand from previous context where you cut off continue from there