---
name: Cluster Issue
about: Report an issue with a cluster
labels: kind/bug

---

**Which cluster is affected**:

  - Dashboard URL
  - Description
  - When the problem started in UTC or hours, e.g. 2018-11-01T15:00:00Z or 3h
  - Priority (inform about pager duty for blocker issues and that people may be woken up behind the scene)

**Shoot:** [garden-berlin/backup](https://dashboard.garden.canary.k8s.ondemand.com/namespace/garden-berlin/shoots/backup)
**Kind:** gcp / europe-west1
**Seed:** [gcp-eu1](https://dashboard.garden.canary.k8s.ondemand.com/namespace/garden/shoots/gcp-eu1)
**Created At:** 2020-06-02
**Last Operation:** ` Flow "Shoot cluster deletion" encountered task errors: [task "Waiting until Shoot control plane has been reconciled" failed: Error while waiting for ControlPlane shoot--berlin--backup/backup to become ready: extension encountered error during reconciliation: Error deleting controlplane: error while waiting for managed resource containing shoot chart for controlplane 'shoot--berlin--backup/backup' to be deleted: timed out waiting for the condition] Operation will be retried. `
**Last Errors:** ` task "Waiting until Shoot control plane has been reconciled" failed: Error while waiting for ControlPlane shoot--berlin--backup/backup to become ready: extension encountered error during reconciliation: Error deleting controlplane: error while waiting for managed resource containing shoot chart for controlplane 'shoot--berlin--backup/backup' to be deleted: timed out waiting for the condition `
**APIServerAvailable:** ` API server /healthz endpoint responded with success status code. [response_time:2ms] `
**ControlPlaneHealthy:** ` Missing required deployments: [cluster-autoscaler] `
**EveryNodeReady:** ` Not enough worker nodes registered in worker pool 'worker-g3w1r' to meet minimum desired machine count. (0/1). `
**SystemComponentsHealthy:** ` Missing required deployments: [coredns metrics-server vpn-shoot] `


**What happened**:

**What you expected to happen**:

**How to reproduce it (as concisely and precisely as possible)**:

**Anything else we need to know**:

**Help us categorise this issue for faster resolution**:

<!-- First word is category, all consecutive words narrow it down. -->
<!-- Please delete every word that doesn't fit here/from your PoV. -->
/area        audit-logging auto-scaling backup certification control-plane cost delivery disaster-recovery documentation high-availability logging metering monitoring networking os performance quality security storage usability user-management
/component   gardener dashboard documentation
/kind        bug regression post-mortem
/os          garden-linux suse-chost
/platform    alicloud aws azure gcp converged-cloud

**Assess the priority of your issue**:

<!-- Keep the next line if this issue has no high urgency. Delete the line, if you go for a higher priority. -->
/priority normal

<!-- Uncomment the following line, if you believe this is a critical issue OR... -->
<!-- /priority critical -->

<!-- ...uncomment the following line, if this issue has direct customer impact and requires our SRE staff to be paged (at night/on weekends). Use only if business continuity is at risk! -->
<!-- /priority blocker -->
