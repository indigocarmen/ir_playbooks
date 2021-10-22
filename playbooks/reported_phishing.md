---
author: indigocarmen
version: 1.0.0
tags: phishing, spam, email
TTP: T1566
---

# Playbook: Title

## Elevator pitch

Phishing is one of the most impactful techniques that actors use, even today. BEC, Malware, and credential theft are rampant because phishing is so effective. This playbook is designed to give investigators quick paths towards verifying a phishing attack was not successful, and guidance on cleaning inboxes up after detection. 

## Alerts captured

* User Reports
* Email Service Provider (ESP) alerts

## Investigation Question and Incident Response

### Identification
<!-- The first level questions are typically hypotheses which we write as an assertion and in italics -->

1. *There is no security threat, we cannot confirm malicious activity*  
2. *This is generic marketing spam with no malicious intent* 
    * The hyperlinks or attachments included are safe (Check through trusted sources such as VirusTotal, OTX, or your own MISP/Taxii setup). 
        * Dismiss
    * The hyperlinks or attachments are known malicious
        * Escalate 
3. *This email is an attempted Business Email Compromise (BEC), with no malicious code or hyperlinks*
    * The email contains attachments or hyperlinks that are known to be malicious
        * Escalate
4. *This email contains malicious code or hyperlinks*  
    * Escalate

### Containment

### Eradication

### Recovery

### Lessons Learned

Following an impactful incident or investigation always perform a lessons learned with the goal of improving your people, processes, or technology!