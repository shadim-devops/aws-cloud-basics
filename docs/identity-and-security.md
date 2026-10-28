# Identity, Security, and Cost Management

## Objective

Configure a basic AWS environment with role-based access, stronger account security, and cost monitoring.

## IAM Groups and Users

Created three IAM groups:

| Group | Intended access |
| --- | --- |
| `admin` | Administrative tasks |
| `developer` | Development-related tasks |
| `readonly` | View-only access |

Assigned appropriate IAM policies, created users, and added users to the relevant groups. Effective permissions depend on the specific policies attached in the AWS account.

## Account Security

Enabled multi-factor authentication (MFA) for the AWS root user.

Configured AWS CLI access for different IAM identities and verified the active identity using:

```bash
aws sts get-caller-identity --profile <profile-name>
```

Check group memberships with:

```bash
aws iam list-groups-for-user --user-name <user-name> --profile <admin-profile>
```

## Budget Monitoring

Created a monthly AWS budget with alerts to help track and control cloud spending.

## Result

The environment includes IAM groups, users, group memberships, configured CLI access, root MFA, and monthly budget monitoring.

> Note: This document records the activities described in the original project report. Specific policy ARNs, budget thresholds, and user names were not provided, so they are intentionally not invented here.
