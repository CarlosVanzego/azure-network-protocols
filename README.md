<p align="center">
<img src="https://i.imgur.com/Ua7udoS.png" alt="Traffic Examination"/>
</p>

<h1>Network Security Groups (NSGs) and Inspecting Traffic Between Azure Virtual Machines</h1>
This project involves the observation of network traffic to and from Azure Virtual Machines (VMs) using Wireshark, along with the experimentation of Network Security Groups (NSGs) for enhanced network security control. The project aims to gain insights into network behavior and refine network security configurations in an Azure environment. The steps include setting up a monitoring environment with Wireshark on a separate VM, configuring NSG rules on the Azure portal, capturing and analyzing network traffic using Wireshark, and experimenting with NSG rules to observe their impact on network traffic. The project involved scripting languages like PowerShell. The Azure portal and virtual machines served as the primary environments for this project, with Wireshark acting as the network protocol analyzer. <br />




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

- Set up a monitoring environment by configuring a separate virtual machine (VM) to install and configure Wireshark.
- Navigate to the Network Security Group (NSG) resource associated with the target Azure VM(s) to experiment with NSG rules.
- Use Wireshark to capture network traffic by selecting the appropriate network interface on the monitoring VM.
- Analyze the captured packets in real-time or save them for later analysis, leveraging Wireshark's features and filters.
- Modify NSG rules in the Azure portal and observe the impact on network traffic captured by Wireshark to experiment and fine-tune network security policies.

<h2>Actions and Observations</h2>

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Start by setting up a monitoring environment. Create a separate VM or use an existing one to install and configure Wireshark, a popular network protocol analyzer. Ensure that the VM is connected to the same Azure VNet as the target VM(s) whose network traffic you want to observe. Configure the network interface on the monitoring VM to capture network traffic.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
On the Azure portal, navigate to the NSG resource associated with the target VM(s). NSGs act as virtual firewalls, allowing you to define inbound and outbound traffic rules. Experiment with creating and modifying NSG rules to control network traffic. You can specify protocols, ports, and source/destination IP addresses to allow or deny traffic. This allows you to implement fine-grained network security policies.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
Within Wireshark on the monitoring VM, select the network interface that captures traffic and start the packet capture. You can choose to capture traffic from a specific IP address or a range of IP addresses associated with the target VM(s). Analyze the captured packets in real-time or save them for later analysis. Wireshark provides various filters and features to inspect and interpret network traffic, including protocol analysis, packet decoding, and flow analysis.
</p>
<br />

<p>
<img src="https://i.imgur.com/DJmEXEB.png" height="80%" width="80%" alt="Disk Sanitization Steps"/>
</p>
<p>
During the packet capture, you can test and validate the impact of NSG rules on network traffic. Modify the NSG rules associated with the target VM(s) to allow or block specific traffic patterns, and observe the corresponding changes in the captured packets. This experimentation with NSGs allows you to understand and fine-tune network security policies, ensuring the desired level of control and protection for your Azure VMs.
</p>
<br />

By following these steps, you can effectively observe network traffic to and from Azure VMs using Wireshark while experimenting with Network Security Groups to enhance network security and control. This approach provides valuable insights into network behavior and enables you to refine and optimize network security configurations for your Azure environment.
