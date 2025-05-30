### 🛡️ Metasploit: Introduction

**Room:** [Metasploit: Introduction — TryHackMe](https://tryhackme.com/room/metasploitintro)  
**Status:** ✅ Completed  
**Date:** *30 May 2025*

---

### 🎯 Objective  
Learn the fundamentals of the Metasploit Framework, including its core components, module types, payload structure, msfconsole usage, and how to search, set, and run exploits like MS17-010 EternalBlue.

---

### 🗝️ Key Concepts  
- **Exploit** — Code used to take advantage of a vulnerability on a target system.  
- **Payload** — The code run after an exploit succeeds (e.g. reverse shell).  
- **Module** — A Metasploit component for tasks like scanning, exploiting, post-exploitation, etc.  
- **Msfconsole** — The main interface to interact with Metasploit via command line.  
- **Session** — A communication channel between Metasploit and the exploited target.  
- **Context** — The current module or state within Metasploit (e.g. exploit context, meterpreter prompt).  
- **setg vs set** — `setg` stores global values across modules, `set` is context-specific.  
- **Exploit Ranks** — Modules are ranked by reliability: excellent, great, good, normal, etc.  
- **Staged Payload** — Payload split into a small initial stager and a larger stage sent after.  
- **Auxiliary Module** — Non-exploit tools like scanners and brute-forcers.

---

### 🛠️ Tools Used  
- **Metasploit Framework** — The main tool used to find, configure, and launch exploits.  
- **msfconsole** — Command-line interface to Metasploit.  
- **EternalBlue Exploit (MS17-010)** — Used to demonstrate exploit usage and payload delivery.  
- **Meterpreter** — A feature-rich payload that provides control over the target system.  

---

### ⚠️ Challenges Faced  
- Getting familiar with different Metasploit prompts (console, context, meterpreter, shell) was confusing.  
- Understanding the difference between `set`, `setg`, and `unset` required practice.  
- Remembering to reconfigure required parameters each time after switching context took a few tries.

---

### 🧠 What I Learned  
- The Metasploit Framework is modular, flexible, and extremely powerful for offensive work.  
- Not all modules are exploits—there are auxiliary, post, scanner, evasion, etc.  
- You can interact with sessions and background them to manage multiple targets.  
- Commands like `search`, `use`, `set`, `exploit`, `run`, and `sessions` are central to efficient workflow.  
- The difference between inline (`_`) and staged (`/`) payloads (e.g. `shell_reverse_tcp` vs `shell/reverse_tcp`) helps identify payload types.

---

### 🌐 Real-World Application:  
> Metasploit is used by penetration testers and red teamers to automate the discovery, exploitation, and control of vulnerable systems. Tools like `ms17_010_eternalblue` simulate real-world attacks such as WannaCry, and show how attackers gain remote access through known CVEs.

---

### 💭 Reflections:  
- The layered approach (modules > payloads > sessions) makes it easier to structure attacks clearly.  
- I was surprised by how powerful and advanced the Metasploit Framework is, and found it fascinating to see everything it can do. 
