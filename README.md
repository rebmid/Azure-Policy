📘 Azure Policy Library – Cost & Governance Controls

This repository contains Azure Policy definitions designed to improve governance, enforce cost discipline, and audit compliance across Azure environments.

📄 Available Policies
  1. Policy_Append-Cost-Tags.json
    Purpose:
    Automatically appends missing cost-related tags (e.g., CostCenter, Project) to resources.
    Effect:
    Append
    Use Case:
    Ensures consistent tagging for cost allocation, reporting, and FinOps governance.

2. Policy-Audit-Tags.json
  Purpose:
  Audits resources for missing required tags.
  Effect:
  Audit
  Use Case:
  Provides visibility into non-compliant resources without blocking deployments.

3. Policy-Enforce-AHR-SQLVMs.json
  Purpose:
  Enforces Azure Hybrid Benefit (AHB) for SQL VMs.
  Effect:
  DeployIfNotExists or Audit
  Use Case:
  Ensures eligible SQL VMs use hybrid licensing to reduce cost.

4. Policy-Enforce-AllHB-Windows.json
  Purpose:
  Enforces Azure Hybrid Benefit for Windows VMs.
  Effect:
  DeployIfNotExists or Audit
  Use Case:
  Reduces Windows VM licensing cost by ensuring hybrid benefit is applied when allowed.

5. Policy-Enforce-Cost-Tags.json
  Purpose:
  Requires specific cost-related tags (e.g., CostCenter, Project, Environment).
  Effect:
  Deny
  Use Case:
  Blocks resource creation when required cost tags are missing.

📘 How to Use These Policies
Assigning Policies in Azure Portal
  Navigate to Azure Portal → Policy → Assign Policy
  Select the appropriate scope (Management Group or Subscription)
  Upload the JSON file
  Configure required parameters
  Save and evaluate compliance
