<p align="center">
  <img src="https://github.com/onyxvail/alx-system_engineering-devops/blob/d73d5df93b989db5d0e10225264d462fb9f4b191/0x19-postmortem/Postmortem-Alx.png" width="75%" height="75%" alt="Image Description">
</p>


------------------------------------------------------------------------------------------
 # 0x19. Postmortem
------------------------------------------------------------------------------------------

# API Service Outage Postmortem: A Galactic Saga of Techno Troubles  🏴🏴

## Issue Summary - Duration :
The outage struck like a meteor shower on October 20, 2023, from 15:00 to 17:30 (GMT+1).

## Impact:
Our API service faced a disturbance in the Force, making it elusive to 50% of our users. Users attempting to wield the API faced a dark period of downtime and error responses.

## Root Cause:
The culprit behind the cosmic hiccup was a misconfigured rate limiter in the API gateway, wielding its power to block requests like a Sith Lord blocking Jedi attacks.

## Timeline - Detection Time:
The automated monitoring system, acting as our loyal astromech droid, sounded the alarm at 3:00 PM (GMT+1).

## Detection Method:
Automated monitoring systems, our vigilant Jedi sentinels, sensed disturbances in the API force and triggered alerts accordingly.

## Action Taken:
The Jedi Council, in this case, our API Development and Security teams, initiated a probe by delving into API server logs and deciphering traffic patterns. Suspecting a potential surge in malicious requests, akin to a dark side DDoS attack, turned out to be a red herring.

## Misleading Paths:
The initial focus on a DDoS attack was as deceptive as a Sith hologram. Temporary measures, akin to using a lightsaber against the wrong enemy, were taken to block certain IP addresses, unfortunately leading to disruptions for legitimate users.

## Escalation:
The incident was raised to the Jedi High Council, our API Development, and Security teams, for a more profound investigation.

## Resolution:
We unraveled the mystery, exposing the misconfigured rate limiter as the Sith Lord behind the chaos. Swiftly, we adjusted its settings to allow for a higher request threshold, restarted the API gateway, and restored peace to the galaxy by 5:30 PM (GMT+1).

## Root Cause Explanation:
The misconfigured rate limiter, acting like a dark side artifact, wielded its power to block legitimate requests, causing a bottleneck in the API force.

## Resolution Details:
In true Jedi fashion, we restarted the API gateway after aligning the rate limiter settings with the Force. Monitoring alerts, our Force-sensitive allies, were refined for early detection of potential disturbances.

## Corrective and Preventative Measures - Improvements/Fixes:
A regular review of API gateway configurations, akin to Jedi training, should be implemented to identify and rectify potential rate limiter misconfigurations. Employing automated tests, like Jedi simulations, can ensure the scalability of our API service.

## Task List:
Conduct a comprehensive review of rate limiter configurations - become one with the API Force.
Implement automated tests for API request rate limits in the continuous integration pipeline - train our API Jedi.
Enhance monitoring alerts to detect abnormal API traffic patterns more quickly - heighten our Force sensitivity.
Develop and document a response plan for similar incidents - create a playbook for the battles that lie ahead.

# To summarize:
The recent service outage was a tale of misaligned stars in the API galaxy. We swiftly countered the Sith-like misconfigured rate limiter, implementing measures to ensure future serenity in our API Force. To maintain the stability of our API infrastructure, we will continue our Jedi training with regular reviews, proactive monitoring, and the power of automated testing - all essential elements in the ongoing saga of technological balance. May the Code be with us!