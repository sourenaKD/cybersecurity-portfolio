# About Me

I am Sourena Karimdadi, a Master of Cyber Security graduate student at Universiti Malaya and a Computer Engineering graduate with a concentration in Computer Networks and Cyber Security. My core academic and professional passion lies in network security, digital protection, and offensive security assessments. Over the past several years, I have built a strong technical foundation through virtualized laboratory environments, hands-on penetration testing scenarios, and academic research into AI-driven intrusion detection systems, cloud forensics, and IoT security workflows. Whether configuring enterprise Active Directory domains in VMware Workstation to test firewall rules or analyzing network traffic anomalies with Wireshark, I enjoy dissecting how complex systems communicate and where their security boundaries fail. I am committed to bridging theoretical security frameworks with practical threat mitigation to help organizations build resilient, secure digital infrastructures.

---

# Technical Skills

* **Penetration Testing & Vulnerability Assessment (Working Knowledge):** Experience conducting network and web security assessments using OWASP methodologies, Burp Suite, and Nmap. Demonstrated in [Web Application Penetration Testing](./projects/web-app-pentest/) and [Enterprise LAN Penetration Testing](./projects/virtual-lab-lan-pentest/).
* **Network Security & Traffic Analysis (Working Knowledge):** Proficient in TCP/IP and OSI models, DNS, DHCP, routing and switching, firewall rule configuration, and packet analysis using Wireshark. Demonstrated in [Enterprise LAN Penetration Testing](./projects/virtual-lab-lan-pentest/).
* **Operating Systems & Virtualization (Confident):** Hands-on administration across Linux distributions (Kali Linux, Parrot Security OS, Ubuntu) and Windows Server (Active Directory, Group Policy), deployed via VMware Workstation and Docker containers. Demonstrated in [Enterprise LAN Penetration Testing](./projects/virtual-lab-lan-pentest/).
* **Programming & Scripting (Beginner to Working Knowledge):** Python (intermediate scripting for automation and security tasks) and C++ (basic).

---

# Certifications and Training

* **Certificate of Completion – Penetration Testing with Kali Linux (PWK)** | Northwest International University *(Completed: July 2025)*
* **Cisco Networking Academy – CyberOps Associate** | *(In Progress – Target Completion: January 2027)*
* **Docker & Containerization Fundamentals** | Self-directed Hands-on Lab Training *(In Progress – Target Completion: December 2026)*

---

# Projects

### 1. [Local Attack Simulation & Enterprise LAN Penetration Testing](./projects/virtual-lab-lan-pentest/)
Designed and deployed a virtualized enterprise network using VMware Workstation featuring Windows Server Active Directory, custom group policies, and segmented firewall rules, followed by comprehensive Nmap reconnaissance and network-level exploitation.

### 2. [Web Application Penetration Testing & OWASP Assessment](./projects/web-app-pentest/)
Conducted a structured security assessment on a target web application environment using OWASP methodologies, Nmap, and Burp Suite to identify HTTP security header misconfigurations and input validation weaknesses.

---

# Learning Journey

Embarking on the Master of Cyber Security program at Universiti Malaya and completing the labs in **WQE7001 Cyber Security** has significantly refined my approach to structured security engineering and documentation. Prior to this course, my practical work in virtualized environments—such as simulating Denial-of-Service (DoS) traffic in Windows Server labs or testing cryptographic communications—was largely exploratory. Through WQE7001, I transitioned from performing ad-hoc technical tasks to adopting a disciplined, evidence-based workflow that emphasizes reproducibility, operational security, and clear technical reporting.

Two specific areas in this course stood out during my progress. First, designing a structured career pathway and aligning it with foundational security controls helped me map my existing networking background directly to Security Operations Center (SOC) and penetration testing competencies. Second, integrating version control via Git and GitHub with static site generation (Jekyll) taught me how modern security professionals treat documentation and portfolios as code. Learning to sanitize screenshots, strip sensitive metadata, and use `.gitignore` files properly reinforced the principle that data leakage prevention starts with our own public repositories.

During the setup of my multi-machine virtual laboratory for network reconnaissance, I encountered a major connectivity issue where my Kali Linux attack machine could not reach the simulated Windows Server domain controller across the custom VMware host-only subnet, resulting in complete packet loss during initial Nmap host discovery scans. To diagnose the issue, I systematically checked the OSI layers: I verified virtual NIC bindings in VMware Workstation, inspected the IP routing tables on both guest operating systems, and ran Wireshark on the virtual adapter. Wireshark revealed that ARP requests were being broadcast, but responses were blocked by a misconfigured Windows Defender Firewall profile that defaulted the new virtual network interface to a restrictive "Public" profile while also conflicting with a stale DHCP lease. By reassigning the network profile to "Domain/Private," flushing the ARP cache, and configuring static IP addressing alongside explicit inbound ICMP and TCP rules for lab testing, I restored full connectivity and documented the troubleshooting workflow.

Despite my comfort with traditional virtual machines and network scanning, I still find cloud-native security orchestration—specifically securing Kubernetes cluster architectures and automated container forensics—challenging due to the ephemeral nature of containerized workloads. To address this gap, my concrete improvement goal is to build and document a vulnerable microservice lab using Docker and Kubernetes, perform container escape and network policy assessments, and complete the Cisco CyberOps Associate training track by **January 31, 2027**. I will measure this goal by publishing a third full project write-up in this portfolio demonstrating container traffic analysis and remediation, accompanied by my verified course completion badge.

---

# Career Objective

My primary career objective upon completing my first semester in the Master of Cyber Security program is to secure a technical internship or junior specialist role in **Penetration Testing, Security Operations Center (SOC) Analysis, or Cloud & Digital Forensics**. Building on my background in computer networks, Kali Linux penetration testing, and Active Directory lab administration, I aim to contribute immediately to vulnerability assessments, incident triage, and network traffic monitoring. To achieve this goal, my next three concrete steps are:
1. Complete the **Cisco CyberOps Associate** certification track to solidify my incident response and SOC monitoring workflows.
2. Expand my hands-on portfolio with advanced labs focusing on cloud security, Docker/Kubernetes environments, and automated DNS/network anomaly detection.
3. Actively participate in local Capture The Flag (CTF) competitions and cybersecurity industry networking events in Kuala Lumpur to sharpen my real-world problem-solving speed.

---

# Contact Information

* **Email:** [sourenakarimdadi@gmail.com](mailto:sourenakarimdadi@gmail.com)
* **GitHub:** [github.com/sourenaKD](https://github.com/sourenaKD)
* **LinkedIn:** [https://www.linkedin.com/in/sourena-karimdadi-7913903a1?trk=contact-info]
