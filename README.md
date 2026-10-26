# Awesome-Mobile-Agent

# Top Mobile Agent Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Unified Endpoint Management, Mobile Device Security & Field Agent Workflows*  
**Last updated: October 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Mobile Agents**. These tools enable IT teams to manage and secure mobile endpoints—smartphones, tablets, rugged devices, and laptops—while empowering field agents and service desk staff to work securely from anywhere through mobile-first workflows, remote management, and zero-trust access.

**Examples** include ServiceNow Mobile Agent, Microsoft Intune, VMware Workspace ONE (Omnissa), Ivanti Neurons for UEM, Jamf Pro, ManageEngine Endpoint Central, SOTI MobiControl, Scalefusion, IBM Security MaaS360, and Citrix Endpoint Management (the category leaders).

**Open-source emphasis**: This section is expanded with active projects for self-hosted mobile device management and Apple-focused MDM—ideal for homelabs, small businesses, non-profits, and organizations building sovereign mobile endpoint infrastructure without per-device licensing lock-in.

Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

- **[ServiceNow Mobile Agent](https://apps.apple.com/kz/app/servicenow-agent/id1446951408)**  
  Mobile-first app for service desk agents to triage, act on, and resolve requests on the go; supports offline work, native device capabilities (barcode scanning, signature capture, navigation), and out-of-the-box workflows for IT, CSM, HR, Field Services, Security Ops, and ITAM; requires ServiceNow Rome instance or later .

- **[Microsoft Intune](https://learn.microsoft.com/hr-hr/intune/)**  
  Comprehensive endpoint management platform for Windows, Apple, Android, and Linux devices; provides MDM and MAM capabilities including device enrollment, configuration profiles, app protection policies, compliance enforcement, conditional access, and Copilot-powered AI agents for device troubleshooting .

- **[VMware Workspace ONE (Omnissa)](https://www.omnissa.com/platform/unified-endpoint-management/)**  
  Unified endpoint management platform ranked a Leader in the 2026 Gartner Magic Quadrant for Endpoint Management Tools; supports Windows, macOS, iOS, Android, ChromeOS, Linux, rugged devices, and virtual endpoints with cloud-native management, zero-touch onboarding, automated app lifecycle, and intent-based workflow orchestration .

- **[Ivanti Neurons for UEM](https://help.ivanti.com/mi/help/en_us/cld/admin/ivanti/118/all/en-us/MobileIronCloud.pdf)**  
  Unified endpoint management with mobile threat defense (MTD), Apple Declarative Device Management (DDM) support, Android Enterprise app deployment workflows, Passkey attestation, and tiered packaging (Bronze through Platinum) covering secure email, MAM, SSO, and AppConnect for iOS .

- **[Jamf Pro](https://www.jamf.com/lp/jamf-pro-enterprise-mobility-management/)**  
  Enterprise mobility management focused exclusively on Apple devices since 2002; provides zero-touch deployment for iPad, iPhone, Mac, and Apple TV, native OS management preserving user experience, self-service app catalog, and security policy enforcement; trusted by 76,600+ organizations including 7 of the top 10 Fortune 500 .

- **[ManageEngine Endpoint Central](https://www.manageengine.com/au/products/desktop-central/edition-comparison-matrix.html)**  
  Unified endpoint management with MDM for mobile devices (Professional and Enterprise editions), out-of-box enrollment for Android (ZTE, Knox, ABM) and Apple (ABM), kiosk mode, geo-fencing, remote lock/wipe, app provisioning, and OS update management for mobile devices .

- **[SOTI MobiControl](https://www.pl.soti.net/resources/blog/2026/soti-mobicontrol-20261-manage-windows-devices-proactively)**  
  Enterprise mobility management with deep Windows device management capabilities in 2026.1 release; features real-time browser traffic monitoring via SOTI Surf, custom scripting for automated issue resolution, centralized firmware/BIOS updates, and patch rollback with CVE visibility .

- **[Scalefusion](https://play.google.com/store/apps/details?id=com.promobitech.mobilock.pro)**  
  Android-focused MDM and kiosk solution for company-owned and BYOD devices; supports single/multi-app kiosk mode, remote lock/wipe, location tracking with geofences, app management (APK upload, remote install/update), content management, VPN client, and custom branding .

- **[IBM Security MaaS360](https://www.ibm.com/jp-ja/products/maas360/mobile-security)**  
  AI-powered unified endpoint management with MaaS360 Advisor for risk insights and user risk management; provides mobile threat defense covering device compromise, network attacks, phishing, and malicious apps, with DLP and container apps for data protection; manages laptops, desktops, IoT, and non-standard devices alongside mobile .

- **[Citrix Endpoint Management](https://docs.citrix.com/de-de/citrix-endpoint-management/about.html)**  
  Endpoint management with MDM+MAM capabilities, micro-VPN via NetScaler Gateway, MAM SDK for securing iOS and Android apps, and integration with Citrix Virtual Apps and Desktops; supports cloud and on-premises deployment with Exchange ActiveSync connector for secure native email .

## Open-Source GitHub Projects

- **[Cairn-MDM](https://github.com/nickpdawson/Cairn-MDM)**  
  Single-binary, open-source Apple MDM server (MIT-licensed) for homelabs, small businesses, non-profits, and families; embeds the MDM protocol server (NanoMDM), SCEP certificate authority, and admin UI in one Go binary with SQLite database; supports macOS and iOS/iPadOS over-the-air enrollment, configuration profile delivery, and an Apple HIG-inspired web console; no Apple Business Manager account required for the non-ABM path; public beta (v0.x) running in production but pre-1.0 .

### Additional Strong Open-Source Options

- **MicroMDM** — The upstream project that Cairn builds upon; a lightweight MDM server for Apple devices focused on the core MDM protocol, suitable for teams wanting to build custom management workflows.
- **NanoMDM** — A minimal MDM server implementation (part of the MicroMDM ecosystem) that Cairn embeds; useful as a library for developers building Apple device management tools.
- **Fleet** — Open-source device management platform built on osquery (MIT); while primarily focused on macOS, Windows, and Linux endpoint visibility, it can complement mobile management workflows for security and compliance monitoring.

**Frameworks for building custom systems**: Deploy **Cairn-MDM** as a self-hosted Apple MDM foundation for iOS/iPadOS/macOS device enrollment and profile management; extend with the **MicroMDM** ecosystem for custom protocol integrations; and layer **Fleet** for cross-platform endpoint visibility in a sovereign mobile agent infrastructure suitable for small to mid-sized deployments.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Mobile agent platforms handling device and user data must comply with applicable privacy regulations (GDPR, CCPA, etc.) and organizational security policies; MDM enrollment grants significant device control requiring careful consent and data governance.
- Self-hosted open-source solutions for mobile management are significantly limited compared to commercial UEM platforms—Cairn-MDM covers Apple device management but does not provide Android, Windows, or Linux support; organizations with heterogeneous fleets should evaluate commercial options or hybrid approaches.
- Verify license terms for commercial use; Cairn-MDM uses MIT .

---

**Made for IT administrators, mobile security engineers, field service managers, and endpoint architects.**  
Let's make mobile agent management more open, secure, and worker-empowering.
