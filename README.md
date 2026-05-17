# Code Samples

A curated collection of projects spanning cloud infrastructure, security automation, AI agent systems, and systems programming.

---

## Projects

### [NIST-Azure-Terraform](https://github.com/Fz96tw/NIST-Azure-Terraform)
**Terraform · Azure · Security Compliance**

End-to-end Terraform implementation of **NIST SP 800-53 Rev. 5** controls on Azure. Organized into six focused modules — Access Control, Audit & Logging, Encryption, Configuration Management, Networking, Vulnerability Management, and Incident Response — each mapping directly to NIST control families. Enforces least-privilege RBAC, CMK disk/storage encryption, VNet isolation, and Microsoft Sentinel-based incident response, with Azure Policy initiatives locking down configuration drift.

---

### [azure-vnet-template](https://github.com/Fz96tw/azure-vnet-template)
**Terraform · Azure Networking · Observability**

Terraform template for a production-style two-tier Azure networking lab. Provisions a frontend/backend VNet with scoped NSGs, two nginx VMs instrumented with Azure Monitor Agent, NSG flow logs v2 with Traffic Analytics, and Connection Monitor for continuous TCP/ICMP health checks — all feeding into a central Log Analytics workspace. A practical reference for Azure network observability and segmentation patterns.

---

### [jira-code-agent](https://github.com/Fz96tw/jira-code-agent)
**Python · AI Agents · Jira API**

An autonomous multi-agent coding system driven by Jira tickets. A webhook server receives Jira events, an architect agent uses GPT-4o to produce a full technical design and ordered task breakdown, and an executor agent implements each task. Status updates, comments, and outputs are written back to Jira in real time. Includes a one-shot `setup_jira.py` utility that creates the required Scrum project, custom issue types (`Initiative`, `Feature`, `Agent Task`, `Agent Subtask`), and custom fields via the Jira REST API.

---

### [entropyscan](https://github.com/Fz96tw/entropyscan)
**C · Security · Systems Programming**

A low-level disk entropy scanner written in C that reads 512 KB blocks from storage devices and computes Shannon entropy for each block, flagging regions likely containing encrypted or compressed data. Maintains a persistent scan history database to avoid redundant rescans and exposes average entropy trends via shell utilities (`showavg.sh`, `watchavg.sh`). Useful for detecting full-disk encryption, ransomware activity, or compressed volume anomalies.

---

### [proxmoxtf](https://github.com/Fz96tw/proxmoxtf)
**Terraform · Proxmox VE · Home Lab**

Terraform configurations for automating VM provisioning on a Proxmox VE home lab cluster. Defines three VMs across two Proxmox nodes — two thin-provisioned Windows Server 2019 clones and a full Ubuntu 24.04 server — each with individually sized virtio/SCSI disks, DHCP networking, and QEMU guest agent enabled. Demonstrates Infrastructure as Code practices for on-premises hypervisor environments using the Telmate Proxmox provider.

---

*Last updated: May 2026*
