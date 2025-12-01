Policy_Append-Cost-Tags.json

Purpose: Automatically appends cost-related tags (e.g., CostCenter) to resources that do not have them.
Effect: Append
Use Case: Helps maintain tagging consistency for cost allocation and reporting.

Policy-Audit-Tags.json

Purpose: Audits resources for missing required tags.
Effect: Audit
Use Case: Provides visibility into resources that are non-compliant with tagging standards without blocking deployments.

Policy-Enforce-AHR-SQLVMs.json

Purpose: Enforces Azure Hybrid Benefit for SQL VMs to optimize licensing costs.
Effect: DeployIfNotExists or Audit
Use Case: Ensures SQL VMs leverage hybrid licensing benefits where applicable.

Policy-Enforce-AllIB-Windows.json

Purpose: Enforces Azure Hybrid Benefit for all Windows VMs.
Effect: DeployIfNotExists or Audit
Use Case: Reduces Windows licensing costs by applying hybrid benefit.

Policy-Enforce-Cost-Tags.json

Purpose: Requires specific cost-related tags on resources (e.g., CostCenter, Project).
Effect: Deny
Use Case: Blocks resource creation if required tags are missing, ensuring compliance with cost governance.


How to Use. Assign Policies

Navigate to Azure Portal → Policy → Assign Policy.
Select the appropriate scope (Management Group or Subscription).
Upload the JSON file and configure parameters as needed.


Best Practices

Apply policies at management group level for enterprise-wide governance.
Combine multiple policies into initiatives for easier management.
Regularly review compliance reports and adjust policies as needed.
