---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}
## Malware Analysis
  ![Malware Analysis](/images/Malware_Analysis.png)

## Cyber Threat Intelligence
<!-- ![Cyber Threat Analysis](/images/Cyber_Threat_Analysis.png){:height="50%" width="50%"} -->

<div align="center">
    <img src="/images/Cyber_Threat_Analysis.png" width="40%" height="40%">
</div>

  
## Host-based Intrusion Detection
<!-- ![HIPS](/images/HIPS.png){:height="60%" width="60%"} -->

<div align="center">
    <img src="/images/HIPS.png" width="65%" height="65%">
</div>

  
### MITRE ATT&CK based Audit log Analysis
Cyber attacks have recently proliferated, causing damages that cost individuals and companies dearly. Our research focus on discover attack techniques and detect APT in host-based audit logs. We propose a provenance-based intrusion detection method which is designed to correlate the context of data flow and analyze causal relationships to detect multi-stage attacks. Based on the provenance graph, we designed a series of algorithms such as behavior abstraction and semantics inference to detect the attack behaviors (i.e., TTPs) occurring on the system. By exploring the correlation between the attack behaviors, we further discover potential APT attacks that may be hidden in the system. To effectively defend against the complexity and evolving of cyber threats, we also develop an automated method for generating synthesized red team campaigns based on the MITRE ATT&CK framework and the common cyber attacks lifecycle.


