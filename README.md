# Awesome-Cloud-Resource-Scaling-Optimization

## Top Cloud Resource Scaling & Optimization Ecosystem

**Curated List of SaaS Products & Open-Source GitHub Projects**  
*Focused on Kubernetes Cost Optimization, Rightsizing & Automated Resource Management*  
**Last updated: March 2026**

This repository tracks notable **SaaS platforms** and **open-source projects** for **Cloud Resource Scaling & Optimization**. These tools help organizations reduce cloud waste by rightsizing workloads, automating idle-resource shutdown, optimizing Kubernetes bin-packing, and providing cost visibility across multi-cloud environments.

**Examples** include Spot by NetApp, Kubecost, CloudHealth by VMware (Broadcom), Cast AI, Harness Cloud Cost Management, Granulate (Intel), AWS Auto Scaling, Turbonomic (IBM), Densify, and Zoho CloudSpend (the category leaders).

**Open-source emphasis**: This section highlights every major active project for self-hosted cost visibility, Kubernetes autoscaling, and FinOps tooling—ideal for platform engineers, SREs, and organizations seeking transparent, vendor-neutral optimization without percentage-of-spend pricing models.

Contributions welcome! Open an PR to add/update entries. Keep descriptions factual and link to official sites.

## Table of Contents
- [SaaS/Hosted Platforms](#saas-products)
- [Open-Source GitHub Projects](#open-source-github-projects)
- [How to Contribute](#how-to-contribute)
- [Disclaimer](#disclaimer)

## SaaS/Hosted Platforms

| Product | Description | Pricing (Starting) | Free Tier / Trial Limits |
|---------|-------------|-------------------|--------------------------|
| **[Kubecost](https://kubecost.com/)** | Kubernetes cost monitoring and optimization platform. Provides real-time cost allocation, rightsizing recommendations, and savings insights. The Amazon EKS-optimized bundle is available at no additional charge and excluded from the $100K spend limit introduced in Kubecost v3 free tier [citation:2]. | Free tier with $100K spend limit; paid plans via sales | Free tier available with spend cap; enterprise license purchasable via AWS Marketplace or directly [citation:12] |
| **[Harness Cloud Cost Management](https://www.harness.io/)** | AI-driven cloud cost optimization with perspectives, budgets, anomaly detection, and AutoStopping rules. Free Forever plan limited to organizations with **< $250K/year cloud spend**, 2 Kubernetes clusters, and 30-day data visibility [citation:5]. | Free Forever (under $250K/year spend); Enterprise quote-only with four separate SKUs (Cloud Cost Insights, Commitment Orchestrator, AutoStopping, Cluster Orchestrator) [citation:5] | **Free Forever**: < $250K/year cloud spend, 2 K8s clusters, 30-day data retention, AutoStopping rules included [citation:5] |
| **[CloudHealth by VMware](https://www.vmware.com/)** | Multi-cloud cost management and governance platform (Broadcom). Charges **2.2–2.5% of tracked cloud spend** with a **$1,000/month minimum**. CH150K plan at $45,000/annual covers up to $150K/month spend; 12-month minimum commitment [citation:13]. | CH150K: $45,000/year (up to $150K/mo spend, 2.5% rate); higher tiers custom [citation:13] | No free tier; free trial available [citation:3] |
| **[Cast AI](https://cast.ai/)** | Kubernetes cost optimization with automated bin-packing, spot instance management, and rightsizing. Pricing starts at **$200/month per feature** according to Software Advice listing [citation:4]. | From $200/month per feature [citation:4] | Free version available per listing; free trial offered [citation:4] |
| **[Spot by NetApp](https://spot.io/)** | Cloud optimization platform for compute and Kubernetes (Ocean, Elastigroup, Eco). Freemium model with self-serve signup. GOV.UK listing shows **£0.03/unit/month** with free trial (all features, limited to 20 VMs) [citation:1][citation:11]. | £0.03/unit/month (GOV.UK listing); pay-as-you-go available [citation:11] | **Free trial**: all features, 20 VMs, limited support [citation:11]; freemium self-serve [citation:1] |
| **[IBM Turbonomic](https://www.ibm.com/products/turbonomic)** | Application resource management and cloud cost optimization across AWS, Azure, GCP, Kubernetes, and on-premises. Gartner reviewer cited **$800 per VM** for licensing [citation:8]. | ~$800/VM (Gartner Peer Insights citation) [citation:8] | 30-day evaluation available (unlimited accounts/VMs) |
| **[Densify](https://www.densify.com/)** | ML-based cloud and container resource optimization. Provides rightsizing recommendations and savings estimates via API. | Quote-only | No public free tier; demo via sales |
| **[Granulate (Intel)](https://granulate.io/)** | Autonomous workload optimization with zero code changes, reducing CPU usage and latency. For pricing, vendor directs users to contact Intel representatives or check the Pricing tab on granulate.io [citation:6]. | Quote-only via Intel [citation:6] | No public free tier; demo available [citation:6] |
| **[AWS Auto Scaling](https://aws.amazon.com/ec2/autoscaling/)** | Native AWS service for automatically adjusting EC2 capacity based on demand. **No additional charge**—you pay only for the EC2 instances, CloudWatch metrics, and other AWS resources consumed [citation:7]. | **Free** (pay only for underlying AWS resources) [citation:7] | Free forever (service itself has no cost) [citation:7] |
| **[Zoho CloudSpend](https://www.manageengine.com/cloudspend/)** | Multi-cloud cost management for AWS, Azure, and GCP. Features chargebacks, budgets, forecasting, and anomaly detection [citation:30]. Zoho's own app listing notes a limitation: it cannot track Zoho's own Catalyst server expenses [citation:17]. | Free app; paid plans available (ManageEngine product); exact pricing not listed in search results | Free version available; free trial offered (ManageEngine listing) |

## Open-Source GitHub Projects

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Kubecost (Open Source)](https://github.com/kubecost/cost-analyzer-helm-chart)** | [![Stars](https://img.shields.io/github/stars/kubecost/cost-analyzer-helm-chart?style=social&color=white)](https://github.com/kubecost/cost-analyzer-helm-chart/stargazers) | Open-source Kubernetes cost monitoring. Deploys via Helm; provides real-time cost allocation, idle cost identification, and rightsizing recommendations. The foundation for Kubecost's commercial offering. |
| **[KubeSurvival](https://github.com/aporia-ai/kubesurvival)** | [![Stars](https://img.shields.io/github/stars/aporia-ai/kubesurvival?style=social&color=white)](https://github.com/aporia-ai/kubesurvival/stargazers) | Finds the cheapest machine types that can run your Kubernetes workloads (~185 stars). Go-based; analyzes resource requirements against cloud pricing [citation:10]. |
| **[Fadvisor (FinOps Advisor)](https://github.com/gocrane/fadvisor)** | [![Stars](https://img.shields.io/github/stars/gocrane/fadvisor?style=social&color=white)](https://github.com/gocrane/fadvisor/stargazers) | Collection of exporters for cloud resource pricing and billing data. Provides cost allocation insights for containers and Kubernetes resources, guided by FinOps principles [citation:10]. |
| **[Kubecost Disk Autoscaler](https://github.com/kubecost/disk-autoscaler)** | [![Stars](https://img.shields.io/github/stars/kubecost/disk-autoscaler?style=social&color=white)](https://github.com/kubecost/disk-autoscaler/stargazers) | Resizes Kubernetes PersistentVolumes automatically based on Kubecost recommendations. Reduces over-provisioned storage costs [citation:10]. |

### Additional Strong Open-Source Options

| Project | Star Badge | Description |
|---------|------------|-------------|
| **[Valence Manifests](https://github.com/valencenet/valence-manifests)** | [![Stars](https://img.shields.io/github/stars/valencenet/valence-manifests?style=social&color=white)](https://github.com/valencenet/valence-manifests/stargazers) | Rightsizes and autoscales containers intelligently for performance and cost management in Kubernetes. Implements a SLO-based autoscaler [citation:10]. |
| **[KEDA](https://github.com/kedacore/keda)** | [![Stars](https://img.shields.io/github/stars/kedacore/keda?style=social&color=white)](https://github.com/kedacore/keda/stargazers) | Kubernetes Event-driven Autoscaling. Scales workloads (including to zero) based on external metrics like queue depth or cron schedules—reducing idle resource costs. |
| **[Goldilocks](https://github.com/FairwindsOps/goldilocks)** | [![Stars](https://img.shields.io/github/stars/FairwindsOps/goldilocks?style=social&color=white)](https://github.com/FairwindsOps/goldilocks/stargazers) | Kubernetes rightsizing tool from Fairwinds. Provides recommendations for resource requests/limits based on actual usage via Vertical Pod Autoscaler. |

**Frameworks for building custom systems**: Combine **Kubecost OSS** for cost visibility, **KEDA** for event-driven scaling to zero, **Goldilocks** for rightsizing recommendations, and **KubeSurvival** for spot instance selection—creating a fully open-source Kubernetes cost optimization stack without percentage-of-spend SaaS fees.

## How to Contribute

1. Fork the repo.
2. Add/edit entries in `README.md` (follow existing format).
3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.
4. Submit PR with a short explanation.

Star the repo if you find it useful!

## Disclaimer

- This is a **community-curated** list — not exhaustive and not an endorsement.
- Cloud cost optimization tools require broad read access to billing and resource metadata; enforce least-privilege IAM roles and audit data access.
- Percentage-of-spend pricing (CloudHealth at 2.5% with $1K minimum) can become expensive at scale; model total cost against projected cloud spend before committing. Self-hosted open-source tools require ongoing tuning and maintenance to remain effective as workloads evolve.

---

**Made for platform engineers, FinOps practitioners, SREs, and organizations building cost-efficient cloud infrastructure.**  
Let's make cloud resource optimization more open, automated, and cost-transparent.
