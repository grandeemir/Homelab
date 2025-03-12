Project Overview: My SOC Homelab Journey

This SOC homelab is a personal project where I explore cybersecurity concepts and gain hands-on experience with security tools. I am not an expert in this field, but I am sharing what I’ve learned so far and documenting my progress.

The main goal of this project is to:

✅ Understand how a Security Operations Center (SOC) functions.

✅ Set up a basic log monitoring and analysis system.

✅ Learn about Active Directory, firewalls, and endpoint security.

✅ Simulate cyber attacks and analyze security responses.

I built this homelab using Virtual Machine Manager (VMM) and open-source tools like pfSense, Wazuh, and REMnux, along with Windows-based systems for a real-world SOC environment simulation.
1. Introduction

In this guide, I will explain step by step how I built my own SOC (Security Operations Center) homelab environment. This project was created to analyze security incidents, manage logs, and enhance my cybersecurity skills. By integrating both open-source and commercial solutions, I have built an environment that closely resembles a real SOC setup.
2. Technologies and Components Used

My homelab consists of the following components:

    pfSense: Firewall and DHCP server
    Ubuntu Server (Wazuh): Log collection and analysis
    Windows Server (Active Directory, DNS): Authentication and DNS services
    Windows 10 Machines: Log collection and endpoint security testing
    Kali Linux: Penetration testing and attack simulation
    REMnux: Malware analysis

All these components are running as virtual machines on Virtual Machine Manager.
3. Setup Steps
3.1 pfsense Installation

    Download the pfSense ISO and install it as a virtual machine.
    Configure firewall and DHCP settings.
    Set up security rules and policies.

3.2 Active Directory Setup

    Install Windows Server and configure Active Directory Domain Services (ADDS).
    Create user accounts and define group policies.
    Complete DNS configuration.

3.3 Windows Workstation

    Join Windows 10 machines to the domain.
    Install Sysmon and other log collection tools.
    Forward logs to Wazuh.

3.4 Ubuntu server (Wazuh) Installatin

    Install Ubuntu Server and perform basic updates.
    Set up Wazuh SIEM and start collecting logs from Windows machines.
    Analyze logs and monitor security events.

3.5 Kali Linux

    Install Kali Linux and set up essential security tools.
    Perform penetration tests on Windows machines and analyze logs.

3.6 REMnux Setup

    Deploy REMnux as a virtual machine and utilize malware analysis tools.
    Examine malware behavior and analyze system responses.

4. Testing and Results

After completing the setup, I conducted the following tests:

    Verified log flow from Windows machines to Wazuh.
    Simulated attacks from Kali Linux and observed security responses from pfSense and Windows systems.
    Used Sysmon and Wazuh to analyze how attacks were detected.

This homelab provides an excellent practice environment for those who want to become SOC Analysts. In the future, I plan to integrate ELK Stack and additional automation tools.
