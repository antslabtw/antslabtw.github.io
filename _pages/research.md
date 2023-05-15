---
layout: archive
title: 
permalink: /research/
author_profile: true
---

{% if author.googlescholar %}
  You can also find my articles on <u><a href="{{author.googlescholar}}">my Google Scholar profile</a>.</u>
{% endif %}

{% include base_path %}

<span style="color:#AB9278;font-weight:700;font-size:38px"> Malware Analysis </span>
<div align="center">
    <img src="/images/Malware_Analysis.png" width="80%" height="80%">
</div>

### AI-based cybersecurity solution for Malicious Behavior Discovery and Interpretation
<div style= "background:#F0E8E5">
The rise of cyber crime markets has led to the development of sophisticated malware, posing a significant challenge to current defensive technologies. In response to this issue, AI-based malware behavior analysis utilizing deep neural networks has shown promise in achieving scalability and accuracy for various cybersecurity tasks. Our research aims to address this challenge through the development of MAMBA (MITRE ATT&CK-based Malicious Behavior Analysis), which utilizes the MITRE ATT&CK framework as a reference for interpreting malware behavior.  
In MAMBA, the key drivers to discovering MITRE techniques include:  
- Incorporating knowledge from the MITRE ATT&CK framework 
- Considering the relation between resources and API calls
- Leveraging resource dependencies among processes  

The design of the MAMBA neural network includes binding embeddings, resource attention, and group attention to enable the discovery of malicious behaviors in examined malware.  
</p><br><br><br>  

<span style="color:#AB9278;font-weight:700;font-size:38px"> Cyber Threat Intelligence </span> 
<div align="center">
    <img src="/images/Cyber_Threat_Analysis.png" width="40%" height="40%">
</div>

### Cybersecurity Ontology for Understanding and Reasoning Adversary Tactics and Techniques
Cyber threat intelligence (CTI) reports provide an overall picture of the fast-evolving attack scenario with semantic descriptions and lists of manipulated resources, offering valuable information about adversaries. To combat increasingly sophisticated cyber threats, CTI can help cybersecurity analysts handle potential attacks as they are unveiled. However, automated extraction of valuable information from unstructured texts remains an ongoing challenge. To address this issue, we designed an information extraction method and constructed an ontology structure capable of integrating parsed information from CTI reports into each instance. This ontology can be used for potential cybersecurity applications, such as semantic reasoning to identify possible adversary groups. This actionable intelligence can directly facilitate threat detection or threat hunting.  
  
  
  
<span style="color:#AB9278;font-weight:700;font-size:38px"> Host-based Intrusion Detection </span> 
<div align="center">
    <img src="/images/HIPS.png" width="65%" height="65%">
</div>

  
### MITRE ATT&CK based Audit log Analysis
Cyber attacks have recently proliferated, causing damages that cost individuals and companies dearly. Our research focus on discover attack techniques and detect APT in host-based audit logs. We propose a provenance-based intrusion detection method which is designed to correlate the context of data flow and analyze causal relationships to detect multi-stage attacks. Based on the provenance graph, we designed a series of algorithms such as behavior abstraction and semantics inference to detect the attack behaviors (i.e., TTPs) occurring on the system. By exploring the correlation between the attack behaviors, we further discover potential APT attacks that may be hidden in the system. To effectively defend against the complexity and evolving of cyber threats, we also develop an automated method for generating synthesized red team campaigns based on the MITRE ATT&CK framework and the common cyber attacks lifecycle.


