<p align="center">
  <a href="https://github.com/Samuel-Cavada" target="_blank">
    <img src="https://img.shields.io/badge/Back_to_Main_Page-000000?style=for-the-badge&logo=github&logoColor=white" alt="Back to Main Page"/>
  </a>
</p>

<h1 align="center">Discovery Scan for Entire Cyber Range Subnet</h1>

<p align="center">
  <img src="https://img.shields.io/badge/Platform-Cyber%20Range-0078D4?style=for-the-badge&logo=microsoft&logoColor=white" alt="Platform" />
  <img src="https://img.shields.io/badge/Tool-Tenable.io-00B388?style=for-the-badge&logo=tenable&logoColor=white" alt="Tool" />
  <img src="https://img.shields.io/badge/Focus-Asset%20Discovery-orange?style=for-the-badge" alt="Focus Area" />
</p>

---

## Project Objective
> This project demonstrates how to run a discovery scan across an entire subnet within a cyber range environment. The goal is to identify active hosts in the 10.xx.xx.xx/xx network and understand their potential roles and categorization within a larger simulated infrastructure.

---

## Tools & Technologies
- **Platform:** Cyber Range Environment
- **OS:** Mixed (depending on discovered hosts)
- **Tools:** Tenable.io
- **Languages/Scripts:** None

---

## Skills Gained / Focus Areas
- Conducted network-wide asset discovery
- Identified hosts and IP ranges in use within a cyber range
- Practiced tagging discovered assets based on roles or systems
- Strengthened familiarity with network reconnaissance using Tenable

---

## Environment Setup
> A cyber range lab environment was used to simulate an enterprise subnet. The scan was designed to cover the IP range `10.xx.xx.xx/xx`, providing visibility into all assets present within the defined range.

![Environment Setup](https://github.com/Samuel-Cavada/Discovery-Scan-for-Entire-Cyber-Range-Subnet/blob/main/images/DSECRS1.png)

---

## Walkthrough
1. [Step 1: Create Discovery Scan](#step-1-create-discovery-scan)
2. [Step 2: Define Target Subnet](#step-2-define-target-subnet)
3. [Step 3: Analyze and Tag Results](#step-3-analyze-and-tag-results)

---

### Step 1: Create Discovery Scan
- Logged into Tenable.io portal at [https://cloud.tenable.com](https://cloud.tenable.com)
- Created a new scan and selected **Discovery Scan** as the type
  - Navigated to:  
    `Scans → My Scans → Create Scan → Nessus Scanner → Host Discovery`

---

### Step 2: Define Target Subnet

- **Basic Tab**:
  - **Name**: `(e.g., Host Scan)`
  - **Description**: `Quick Description`
  - **Scanner Type**: `Internal Scanner`  
  - **Scanner**: `Auto-select`  
  - **Network**: `entered the full subnet range: 10.xx.xx.xx/xx`  
  - **Target**: `VM’s Public IP`  
- **Save & Launch**

![Step 2](https://github.com/Samuel-Cavada/Discovery-Scan-for-Entire-Cyber-Range-Subnet/blob/main/images/DSECRS7.png)

---

### Step 3: Analyze and Tag Results
- Checked the “Scans” tab in Tenable to view scan status and results:  
  `Scans → My Scans → Your Agent Scan Name → See All Details`
- Reviewed all discovered hosts
- Considered each system’s potential purpose based on IP, hostname, or service banner  
- Tagged assets by categories such as “Workstation,” “Server,” or “Unknown” as applicable

![Step 3](https://github.com/Samuel-Cavada/Discovery-Scan-for-Entire-Cyber-Range-Subnet/blob/main/images/DSECRS13.png)
![Step 3](https://github.com/Samuel-Cavada/Discovery-Scan-for-Entire-Cyber-Range-Subnet/blob/main/images/DSECRS14.png)

---

## Outcomes and Lessons Learned
- **Technical Insight:** Discovery scans provide visibility into unknown or undocumented assets within a network—essential for strong asset inventory.
- **Configuration Skills:** Gained experience setting up subnet-wide scans and identifying IP range characteristics.
- **Troubleshooting:** Some hosts may not respond to pings or may have firewalls blocking scans; consider refining techniques to ensure better coverage.
- **Takeaway:** A successful discovery scan is the first step toward comprehensive vulnerability management by building an accurate asset inventory.

---

## References
- [Tenable Discovery Scans Guide](https://docs.tenable.com/nessus/Content/DiscoveryScan.htm)
- [CIDR Subnet Reference](https://www.ipaddressguide.com/cidr)
- [Tenable.io Documentation](https://docs.tenable.com/)
