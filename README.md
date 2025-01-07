<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
In this tutorial, we observe various network traffic to and from Azure Virtual Machines with Wireshark as well as experiment with Network Security Groups. <br />


<h2>Video Demonstration</h2>

- ### [YouTube: Azure Virtual Machines, Wireshark, and Network Security Groups](https://www.youtube.com)

<h2>Environments and Technologies Used</h2>

- Microsoft Azure (Virtual Machines/Compute)
- Remote Desktop
- Various Command-Line Tools
- Various Network Protocols (SSH, RDH, DNS, HTTP/S, ICMP)
- Wireshark (Protocol Analyzer)

<h2>Operating Systems Used </h2>

- Windows 10 (21H2)
- Ubuntu Server 20.04

<h2>High-Level Steps</h2>

- Set Up Virtual Machines

Create two Azure VMs (Windows and Ubuntu) in the same virtual network for testing network protocols.
- Configure Network Security Groups (NSGs)

Set up NSG rules to control inbound and outbound traffic for each VM, specifying protocols and ports.
- Capture and Analyze Traffic

Use Wireshark on the Windows VM to monitor and capture network traffic. Test connectivity between VMs to analyze the effects of NSG rules.
- Adjust NSG Rules and Document Observations

Modify NSG rules to allow or block specific traffic, observe the impact, and document findings.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Set Up Azure Virtual Machines

Create two VMs in the same virtual network: one running Windows 10 and the other running Ubuntu Server 20.04.
Configure Network Security Groups (NSGs)

Navigate to the Azure portal and create an NSG.
Define inbound and outbound security rules to control traffic flow. For example, allow RDP (port 3389) for Windows and SSH (port 22) for Ubuntu.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Install Wireshark on the Windows VM

Download and install Wireshark on the Windows VM to monitor network traffic.
Capture Network Traffic

Use Wireshark to capture traffic on the Windows VM.
Initiate various network communications (e.g., ping, SSH, HTTP) between the two VMs and observe the captured packets.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Analyze Traffic Based on NSG Rules

Modify NSG rules to allow or deny specific traffic types.
Observe how changes in NSG rules affect the network traffic captured by Wireshark.
Document Observations

Record the impact of different NSG configurations on network traffic.
Note any unexpected behaviors or insights gained during the analysis.
</p>
<br />
