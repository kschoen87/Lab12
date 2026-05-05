Lecture 25 introduced forensic discipline: chain of custody, evidence integrity, the Pyramid of Pain, IOCs, and the Easttom Ch 16 framework for investigating an event after the fact. Lab 12 is where that framework stops being slides and starts being a real triage workflow you walk through end to end.

You receive one Sysmon EVTX file from a workstation you have never touched, handed to you as evidence with the host already isolated. Your job is to verify the file’s integrity, document a chain of custody as you analyze it, identify what the adversary did, extract Indicators of Compromise (IOCs) and classify each by Pyramid of Pain tier, map the activity to MITRE ATT&CK techniques, and produce a half-page triage memo for the requesting party.

This is the only forensic hands-on you get this term. Lab 13 (assigned at the same time) covers the live SOC operational view; P03 builds on that operational stack. Forensics is its own discipline, and the toolchain reflects that: native Windows Event Viewer plus PowerShell, not Splunk. Forensic investigation and live SOC operations are different skill sets that share telemetry but use different tools. Take the workflow seriously.

By the end of this lab you will have:

A verified evidence bundle in a known-good state on your Windows VM, with the chain of custody documented from the moment of receipt
A working understanding of how Event Viewer + PowerShell Get-WinEvent + Get-FileHash form a forensic triage toolkit
An IOC table extracted from a real Sysmon EVTX, classified by Pyramid of Pain tier
An ATT&CK technique mapping tied to the evidence
A half-page triage memo that would not embarrass you to send to a client
Format: Hands-on. Assigned Thursday, April 23 (paired with Lab 13). Due and locked Tuesday, May 5 at 11:59 PM.

Why this lab exists: the rest of the term’s detection / monitoring content focuses on live operational defense (Lab 13, P03). That’s where the bulk of SOC work happens, but it is not the whole picture. Forensics is the discipline you reach for when something has already happened and you have to reconstruct it from artifacts. Every defender needs to have done it once. Lab 12 is that once.

What you’ll learn:

How to verify evidence integrity with cryptographic hashes and reject corrupted bundles
How to maintain chain of custody as a real working artifact, not bureaucratic ceremony
How to triage a Sysmon EVTX file using Windows Event Viewer + PowerShell — the same Sysmon channel you’ll be ingesting in Lab 13, examined offline
How to extract IOCs from event logs and classify them by Pyramid of Pain tier with defensible reasoning
How to map observed activity to MITRE ATT&CK techniques with evidence backing each mapping
How to write a tight forensic triage memo that respects a busy reader’s time
Relevant SLOs:

SLO 9: Detect and remove malware from computer systems
SLO 10: Detect malicious activity in computer systems and networks
