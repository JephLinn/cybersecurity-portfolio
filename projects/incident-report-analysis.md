**Incident report analysis**

**Instructions**

As you continue through this course, you may use this template to record your findings after completing an activity or to take notes on what you've learned about a specific tool or concept. You can also use this chart as a way to practice applying the NIST framework to different situations you encounter.

| Summary | Earlier today, our internal network was compromised for two during a DDoS attack, specifically an ICMP flood. Our network stopped responding due to the flood of ICMP packets, and the normal internal network couldn’t access any network resources. Our incident management team responded by blocking the incoming packets, halting all non-critical network services offline while restoring critical services. |
| :---- | :---- |
| Identify | It appears the malicious actor sent a flood of ICMP packets through an unconfigured firewall. This let the malicious actor overwhelm the network with a DDoS attack the whole network was shutdown and all users lost access. |
| Protect | The network security team implemented the following measures: A new rule to the firewall limiting the rate of the incoming ICMP packets. The use of an IDS/IPS system to filter out traffic with suspicious traits. |
| Detect | Checking for spoofed IP addresses on incoming ICMP packets via source IP address verification on the firewall. Using a SIEM tool to monitor software and detect abnormal traffic patterns. |
| Respond | In the future, we will isolate affected system to minimize attack surface. We will use network logs to analyze log to check for abnormal activity. |
| Recover | Future attacks can be blocked by our reconfigured firewall. During this kind of attack, the goal is to restore normal network functionality. By stopping all non-critical network services offline we can reduce network traffic.  Restoring critical services is the first step followed by the rest. |

---

| Reflections/Notes: |
| :---- |

