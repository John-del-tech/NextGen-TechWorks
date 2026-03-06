# README

## Report overview

This repository contains the report IT Infrastructure Upgrade for NextGen Tech Works. NextGen TechWorks is a small-to-medium enterprise that provides gaming stations for professionals and enthusiasts. The report is written as a Personal Learning Record covering Weeks 1 to 12. It documents component selection, system unit planning, storage and peripherals evaluation, SME network design, DHCP and DNS configuration, project management planning, cyber security controls, troubleshooting records, operating system setup, mobile device and IDE protocols, and cloud and virtualisation evaluation. The report includes 21 Harvard Solent references and uses appendices to present supporting charts, tables, and project artefacts.

## Folder structure

Diagrams
Contains the three figures referenced in the appendices:
Figure 1.Throughput vs offered load in mixed 802.11ax802.11ac networks (Natkaniec and Bieryt, 2023).png
Figure 2. Docker vs host execution time comparison (Kononowicz and Czarnul, 2022).png
Figure 3. NextGen TechWorks (SME) - Site Network and Cloud Integration.png

Report
Contains the main report content, including weekly task summaries and the reference list.

## Appendices content

### Appendix A. Charts and Tables

**Figure 1**
*Throughput versus offered load in mixed IEEE 802.11ax and IEEE 802.11ac networks, with and without BSS coloring (Natkaniec and Bieryt, 2023).*
![Figure 1. Throughput vs offered load in mixed 802.11ax/802.11ac networks (Natkaniec and Bieryt, 2023)](Diagrams/Figure%201.Throughput%20vs%20offered%20load%20in%20mixed%20802.11ax802.11ac%20networks%20(Natkaniec%20and%20Bieryt,%202023).png)

**Figure 2**
*Docker versus host execution time comparison for parallel computing workloads across increasing numbers of processes (Kononowicz and Czarnul, 2022).*
![Figure 2. Docker vs host execution time comparison (Kononowicz and Czarnul, 2022)](Diagrams/Figure%202.%20Docker%20vs%20host%20execution%20time%20comparison%20(Kononowicz%20and%20Czarnul,%202022).png)

**Table 1**
*Key gaming-station component shortlist and selection rationale.*
+-----------+------------------------------+----------------------------------------------+--------------------+
| Component | SME gaming-ready             | Why it is selected                           | Budget             |
|           | specification                |                                              | note               |
+-----------+------------------------------+----------------------------------------------+--------------------+
| CPU       | 8-16 cores, high single-     | Supports high FPS plus                        | Mid-high           |
|           | thread boost                 | streaming/creation workloads                  | cost driver        |
+-----------+------------------------------+----------------------------------------------+--------------------+
| GPU       | Current gen, 12-16 GB        | Enables high-resolution gaming                | Highest cost       |
|           | VRAM (or higher)             | and pro graphics tasks                        | item               |
+-----------+------------------------------+----------------------------------------------+--------------------+
| RAM       | 32-64 GB DDR4/DDR5           | Stable multitasking, IDEs,                    | Scale with         |
|           |                              | streaming tools                               | users              |
+-----------+------------------------------+----------------------------------------------+--------------------+
| Storage   | 1-2 TB NVMe SSD +            | Fast load times plus capacity for             | Tiered             |
|           | optional HDD/NAS             | media/projects                                | spend              |
+-----------+------------------------------+----------------------------------------------+--------------------+

**Table 2**
*Network and cloud options mapped to NextGen operational needs and cost control approach.*
+--------------+---------------------------+----------------------------------------------+--------------------+
| Area         | Selected solution         | Business value for NextGen                   | Cost control       |
|              |                           | SME                                          | approach           |
+--------------+---------------------------+----------------------------------------------+--------------------+
| LAN core     | Managed switch +          | Separates admin, guest, and                  | Buy once, multi-   |
|              | VLANs                     | gaming traffic                               | year use           |
+--------------+---------------------------+----------------------------------------------+--------------------+
| Wi-Fi        | Wi-Fi 6 (802.11ax)        | Better throughput under load,                | Right-size AP      |
|              | APs                       | improved efficiency                          | count              |
+--------------+---------------------------+----------------------------------------------+--------------------+
| Core         | DHCP/DNS on server        | Reliable addressing + name                   | Use existing       |
| services     | or firewall               | resolution                                   | licences           |
+--------------+---------------------------+----------------------------------------------+--------------------+
| Cloud        | Cloud backup or           | Scalability and resilience                   | Pay only for       |
|              | hybrid storage            |                                              | usage              |
+--------------+---------------------------+----------------------------------------------+--------------------+

### Appendix B. Project Artifacts

**Figure 3**
*NextGen TechWorks (SME) site network and cloud integration diagram.*
![Figure 3. NextGen TechWorks (SME) site network and cloud integration diagram](Diagrams/Figure%203.%20NextGen%20TechWorks%20(SME)%20-%20Site%20Network%20and%20Cloud%20Integration.png)

**Table 3**
*Project plan: Timeline and deliverables (by week).*
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| Week(s) | Work package                  | Key activities                                                 | Outputs for PLR evidence                                      |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 1       | PC components                 | Research CPU, GPU, motherboard options; compare                | Component shortlist table                                     |
|         |                               | benchmarks/specs; check compatibility and upgrade paths         | + justification notes + cost estimates                        |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 2       | System unit components        | Select cooling and PSU; validate power draw and efficiency;     | Compatibility checklist                                       |
|         |                               | confirm case airflow assumptions                                | + PSU sizing notes + updated cost table                       |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 3       | Storage and power strategy    | Compare NVMe SSD vs SATA SSD vs HDD; define storage tiers for   | Comparison chart                                              |
|         |                               | gaming rigs and shared files; confirm backup approach           | + recommendation table + budget update                        |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 4       | Peripherals and external      | Select monitor, keyboard, mouse, headset, printer; define       | Images with sources                                           |
|         | devices                       | maintenance and replacement schedule                            | + setup/maintenance notes + peripheral cost table             |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 5       | Networking design             | Design SME network layout; select switch/AP/router; define      | Network diagram (PlantUML)                                    |
|         |                               | VLANs for gaming, admin, guest                                  | + hardware quotes + design rationale                          |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 6       | Protocols and services        | Plan and document DHCP/DNS; define IP scheme; test connectivity | Configuration screenshots/logs                                |
|         |                               | and name resolution                                             | + simple performance checks                                   |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 7       | Project management            | Confirm roles, timeline, dependencies; introduce change control | Short Gantt-style schedule                                    |
|         |                               | and risk tracking                                               | + roles list + risk register summary                          |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 8       | Cyber security                | Define baseline security controls (accounts, MFA, patching,      | Risk matrix                                                   |
|         |                               | backups, endpoint protection, firewall rules); perform risk     | + security checklist + audit evidence screenshots             |
|         |                               | assessment                                                     |                                                               |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 9       | Troubleshooting               | Record issues encountered and fixes (hardware, drivers, network, | Troubleshooting diary table                                   |
|         |                               | latency, updates)                                              | + resolution summaries + tool outputs                         |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 10      | Operating systems             | Select OS edition; document install, updates, drivers, policies; | OS setup evidence                                             |
|         |                               | apply security hardening                                        | + configuration screenshots + verification outputs            |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 11      | Mobile devices and IDEs       | Define mobile management rules; enforce lock screen and MFA;     | Policy notes                                                  |
|         |                               | document IDE setup for productivity workflows                   | + setup steps + screenshots showing configurations            |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
| 12      | Cloud and virtualisation      | Choose cloud service model for backup/monitoring; document       | Cloud plan summary                                            |
|         |                               | virtualisation or container plan; evaluate impact               | + performance notes + final budget totals                     |
+---------+-------------------------------+---------------------------------------------------------------+---------------------------------------------------------------+
