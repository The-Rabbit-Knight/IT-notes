# The Diamond Model

The **Diamond Model** is a framework used in cybersecurity to analyze intrusions.  
It represents the relationship between **adversary, infrastructure, capability, and victim**. 
Used in incident response and threat intel to map out relationships and patterns. Helps attribute attacks and understand adversary behavior.

---

## The Four Core Features
1. **Adversary** – the threat actor or group responsible for the intrusion.  
2. **Infrastructure** – the tools, servers, or resources they use.  
3. **Capability** – the malware, exploits, or attack techniques.  
4. **Victim** – the target organization, system, or person.
These four points form a *diamond shape*, showing how each feature relates to the others.

The distinction between an adversary operator and an adversary customer is essential for understanding the intent, attribution, adaptability, and persistence of an attack. 
This distinction helps to frame the relationship between the attacker and the victim. Utilizing data from an incident or breach, along with signatures and other relevant information, can help determine the identity of the adversary.

**Adversary Operator**: This is the "hacker" or the individual(s) who are actively conducting the intrusion activity. They are the ones who execute the technical actions of the attack.
**Adversary Customer**: This is the entity that stands to benefit from the intrusion. This could be the same person or group as the adversary operator, or it may be a separate person, group, or organization that hires the operator to carry out the attack.

An attacker's capability refers to the skills, tools, and methods they use in an attack. It's how they get from a plan to a finished attack. This includes everything, from simple tricks like guessing passwords to complex actions like writing their own malware.
The **capability capacity** is all the possible ways that a specific skill or tool could be used. Think of it as the full potential of that one capability. For example, the capacity of a password-guessing tool would be all the different usernames and passwords it could try.
An **Adversary Arsenal** is the total collection of all the different capabilities an attacker has. It’s a list of all their skills and tools. The combined capacity of an attacker’s entire arsenal is the total of all the different things they can do.

---

## Visual Representation

```
           Adversary
              / \
             /   \
   Capability     Infrastructure
             \   /
              \ /
            Victim
```
---
## Why It’s Useful
- Helps analysts **connect different intrusion events**.  
- Provides a structured way to **pivot investigations**.  
- Makes it easier to **share intelligence** with others.

---

##  Additional Meta-Features

| Meta-Feature    | Description | Example / Notes |
|-----------------|-------------|----------------|
| **Timestamp**   | When the event occurred (start/end). Helps spot patterns. | Attack at 2 AM US → attacker may be in another time zone. |
| **Phase**       | Stage of the attack. Most attacks happen in sequential steps. | Follows Cyber Kill Chain |
| **Result**      | Outcome of the event. Can be success, failure, or unknown; may affect Confidentiality, Integrity, or Availability. | "Confidentiality breached," "Integrity compromised," stolen credentials. |
| **Direction**   | Flow of the attack between entities. | Victim→Infra, Infra→Victim, Infra→Infra, Adversary→Infra, Infra→Adversary, Bidirectional, Unknown. |
| **Methodology** | Type of attack or technique used. | Phishing, DDoS, breach, port scan, malware. |
| **Resources**   | External assets used to carry out the attack. | Software (OS, Metasploit), knowledge, credentials, hardware, funds, facilities, network access. |

---
