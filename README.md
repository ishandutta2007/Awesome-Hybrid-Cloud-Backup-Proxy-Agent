# Top Hybrid Cloud Backup Proxy & Agent
**Curated List of SaaS Products & Open-Source GitHub Projects**

*Focused on Backup Proxies, Media Agents, Endpoint Agents, Hybrid Cloud Data Protection & Distributed Backup Architecture*

**Last updated: November 2026**

This repository tracks notable **SaaS / commercial platforms** and **open-source projects** for **Hybrid Cloud Backup Proxies and Agents**. These components act as intermediaries or local agents that move, process, deduplicate, and transfer backup data between on-premises systems and cloud or secondary storage targets.

**Examples** include Druva Backup Proxy, Veeam Backup Proxy, Commvault MediaAgent, Cohesity Cloud Edition, Acronis Backup Agent, Rubrik Edge, Datto Endpoint Backup Agent, Quest Rapid Recovery Core, NAKIVO Transporter, and Arcserve UDP Agent (the category leaders).

**Open-source emphasis**: While commercial backup platforms dominate enterprise hybrid deployments with polished proxies and media agents, strong open-source alternatives exist. **Bareos**, **Bacula**, **UrBackup**, **Proxmox Backup Server**, **Restic**, **BorgBackup**, **Kopia**, and related projects provide client/server or agent-based architectures suitable for hybrid cloud backup workflows. This section is heavily expanded.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-hosted-platforms)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Starting Price | Free Tier / Trial Limits |
| :--- | :--- | :--- | :--- |
| **[Druva Backup Proxy](https://www.druva.com/)** | Cloud-native backup proxy component that enables efficient data movement from on-premises workloads into Druva’s SaaS data protection platform. | Starting at ~$8.00/user/month (or consumption-based per TB post-dedup) | 30-day free trial (no credit card required, full functionality across evaluation workloads) |
| **[Veeam Backup Proxy](https://www.veeam.com/)** | Core transport component in Veeam Backup & Replication that handles data movement, compression, and deduplication between sources and backup repositories (including cloud targets). | Starting at ~$95/workload/year (Veeam Data Platform Essentials 5-pack bundle at ~$428/year) | Free forever Community Edition up to 10 workloads; 30-day full-featured enterprise trial |
| **[Commvault MediaAgent](https://www.commvault.com/)** | MediaAgent serves as the data mover and storage handler in Commvault environments, managing backup traffic between clients, on-prem storage, and cloud repositories. | Starting at ~$1.70/user/month for SaaS apps; ~$58.50/TB/month for file/object workloads (~$98/VM/year) | 30-day free trial with full SaaS platform access (or 30,000 trial credits on hyperscaler marketplaces) |
| **[Cohesity Cloud Edition / Agents](https://www.cohesity.com/)** | Hybrid components and agents that integrate on-premises data sources with Cohesity’s cloud and secondary storage platforms. | Starting at ~$29,100/year for baseline BaaS packages (~10 BETB entry commitment on AWS Marketplace) | 30-day free trial for Backup-as-a-Service (DataProtect) |
| **[Acronis Backup Agent](https://www.acronis.com/)** | Endpoint and workload agents that protect physical, virtual, and cloud systems and move data into Acronis Cyber Protect storage targets. | Starting at ~$85/workstation/year and ~$595/server/year | 30-day full-featured free trial |
| **[Rubrik Edge](https://www.rubrik.com/)** | Lightweight edge component that extends Rubrik’s data management platform to remote or edge locations for hybrid backup and recovery. | Starting at ~$3.80/user/month for cloud apps; enterprise platform contracts typically start around ~$50,000/year | 30-day free trial for specific SaaS modules (e.g., Salesforce); custom PoC/demo for core Edge platform |
| **[Datto Endpoint Backup Agent](https://www.datto.com/)** | Agent used in Datto’s endpoint and hybrid backup solutions for continuous or scheduled protection of endpoints and servers. | Starting at ~$105/month for packaged DR configurations (or ~$2–$6/endpoint/month via MSP tiers) | Free partner NFR evaluation licenses (2 free NFR PC licenses for registered partners); guided trial spin/demo for prospects |
| **[Quest Rapid Recovery Core](https://www.quest.com/)** | Core/engine component that manages replication, backup, and recovery operations across hybrid environments. | Starting at ~$1,819.99/license (includes 1 year of 24x7 support & maintenance) | 14-day free trial (extendable by administrators up to 28–30 days) |
| **[NAKIVO Transporter](https://www.nakivo.com/)** | Data mover component in NAKIVO Backup & Replication responsible for transferring backup data between sources, proxies, and repositories. | Starting at ~$2.45/workload/month (or perpetual licenses from ~$229/socket) | Free forever Edition for up to 10 workloads + 5 M365 users; 15-day unconstrained full trial |
| **[Arcserve UDP Agent / Proxy](https://www.arcserve.com/)** | Agents and proxy roles within Arcserve Unified Data Protection for hybrid backup, replication, and recovery workflows. | Starting at ~$19.99/front-end TB/month (or annual software subscriptions from ~$1,300/year) | Free forever Workstation Free Edition (after trial); 30-day full-featured free trial |

## Open-Source GitHub Projects
- **[Bareos](https://github.com/bareos/bareos)**  
  Fully open-source (AGPLv3) cross-network backup solution with Director, Storage Daemon, and File Daemon architecture. Closest open equivalent to commercial proxy/media-agent designs; supports disk, tape, and S3-compatible storage.

- **[Bacula Community](https://www.bacula.org/)**  
  Classic open-source network backup system (Director + Storage Daemon + File Daemon). Provides enterprise-style catalog, scheduling, and multi-client protection suitable for hybrid environments.

- **[UrBackup](https://github.com/uroni/urbackup_backend)**  
  Open-source client/server backup system with web UI. Supports both file and image backups for Windows and Linux clients, making it practical for smaller hybrid deployments.

- **[Proxmox Backup Server](https://github.com/proxmox/proxmox-backup)**  
  Dedicated open-source backup server optimized for Proxmox VE and other workloads. Offers client-side encryption, deduplication, and efficient hybrid storage targets.

- **[Restic](https://github.com/restic/restic)**  
  Modern, fast, encrypted backup tool written in Go. Excellent for hybrid cloud use cases with native support for S3, SFTP, REST server, and many other backends via rclone.

- **[BorgBackup](https://github.com/borgbackup/borg)**  
  Deduplicating, compressing, and encrypting backup program. Widely used for efficient server-to-server or server-to-cloud hybrid backup pipelines over SSH.

- **[Kopia](https://github.com/kopia/kopia)**  
  Cross-platform open-source backup tool with CLI and GUI. Supports encryption, deduplication, and multiple cloud/object storage backends for hybrid scenarios.

- **[Duplicati](https://github.com/duplicati/duplicati)**  
  Free, open-source backup client with a web UI. Works well for endpoint and small-server hybrid backups to cloud storage providers.

- **[Rclone](https://github.com/rclone/rclone)**  
  Extremely versatile open-source command-line tool for syncing and transferring data to/from cloud storage. Frequently used as a transport or “proxy-like” layer in hybrid backup scripts.

- **[Amanda](https://www.amanda.org/)**  
  Long-standing open-source network backup system that can coordinate backups across multiple clients to centralized storage, including cloud targets.

### Additional Strong Open-Source Options
- Enterprise-style client/server (proxy/agent model): **Bareos**, **Bacula Community**, **UrBackup**.
- Modern encrypted file-level tools ideal for hybrid cloud: **Restic**, **BorgBackup**, **Kopia**.
- Backup server focused: **Proxmox Backup Server**.
- Transport / sync layer: **Rclone**.
- Accepting that commercial solutions (Veeam Backup Proxy, Commvault MediaAgent, Druva, Rubrik Edge, NAKIVO Transporter, Acronis agents) still lead in enterprise features such as advanced application awareness, instant recovery, global deduplication scale, and vendor support.

**Frameworks for building custom systems**:  
Deploy **Bareos** or **Bacula** File Daemons as agents and Storage Daemons as proxies → use **Restic** or **BorgBackup** for efficient encrypted transfers to S3-compatible or object storage → orchestrate with scripts or **Rclone** for additional cloud mobility. Ideal for teams that want full control, data sovereignty, and no per-agent licensing costs in hybrid environments.

## How to Contribute
1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer
- This is a **community-curated** list — not exhaustive and not an endorsement.
- Backup and recovery systems are critical infrastructure. Always validate restore procedures, test recovery time/point objectives, and review encryption, retention, and compliance requirements. Open-source tools offer transparency and cost advantages but place more responsibility on the operator for configuration, monitoring, and support. This list is not professional backup, disaster recovery, or compliance advice.

---
**Made for backup administrators, infrastructure engineers, and open-source advocates.**

Let's keep hybrid data protection powerful, transparent, and under your control.
