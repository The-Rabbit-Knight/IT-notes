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

---

## Visual Representation

         Adversary
           / \
          /   \
Capability --- Infrastructure
          \   /
           \ /
         Victim
---

##  Additional Meta-Features
- **Timestamp** – when the activity occurred.  
- **Phase** – which phase of the intrusion (planning, exploitation, etc.).  
- **Result** – the outcome of the attack.  

---

## Why It’s Useful
- Helps analysts **connect different intrusion events**.  
- Provides a structured way to **pivot investigations**.  
- Makes it easier to **share intelligence** with others.

--- 

# Diamond Model Example

| Element            | Description                                              | Example                                                                             |
|--------------------|----------------------------------------------------------|-------------------------------------------------------------------------------------|
| **Adversary**      | The threat actor performing the attack.                  | Allegedly Russian state actors (Sandworm, APT28).                                   |
| **Capability**     | The tools/malware/exploits used.                         | Compromised MeDoc update servers, spread via SMB, PsExec.                           |
| **Infrastructure** | C2 servers, phishing domains, email infrastructure, etc. | Modified ransomware wiper, EternalBlue exploit, Mimikatz.                           |
| **Victim**         | The targeted person or organization.                     | Ukrainian companies, and eventually global organizations like Maersk, Merck, FedEx. |


