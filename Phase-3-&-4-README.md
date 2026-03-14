
<h2>Description</h2>
This phase operationalizes the detection rules I built in Phase 3. The goal is to make Splunk behave like a real SOC tool, not just search, but alert and visualize.
<br />

<h2>  Brute Force SSH with Hydra </h2>

- SSH brute force is the most common attack against Linux hosts and generates clean, readable logs. 
<br /> 
<br />
<img src="https://imgur.com/ArJkl2H.jpg"  height="80%" width="80%">
<img src="https://imgur.com/ZDrzpyY.jpg"  height="80%" width="80%">
<br />

- Searches all indexes for failed SSH password events from Linux auth logs.
- Aggregates the count of failures, grouped by source IP and username.
- Filters to only show IPs/users with more than 5 failures (brute force threshold).
- Sorts results highest count first, so the worst offenders appear at the top.

<br />
<img src="https://imgur.com/GqMHCwL.jpg"  height="80%" width="80%">


<br />
