# SIG Observability Charter

This charter adheres to the conventions described in the [Kubernetes Charter README] and uses
the Roles and Organization Management outlined in [sig-governance].

## Scope

SIG Observability is responsible for the components that make Cluster Operation and Maintenance decisions.
We build Kubernetes observabilty features for Kubernetes Ecology. We design and
implement features that allows users to collect, store, monitor, aggregate, alert of Resources on the nodes
of muti-cluster. These features include those that improve reliability of workloads,
more efficient use of cluster resources, and/or enforces placement policies. 

### In scope

SIG [readme]

#### Code, Binaries and Services

- Network collect (e.g. [Pingmesh exporter](https://github.com/kubeservice-stack/pingmesh-agent))
- Kernel collect (e.g. [eBPF exporter](https://github.com/kubeservice-stack/ebpf_exporter))
- Observability stack (e.g. [OPSCenter](https://github.com/kubeservice-stack/OpsCenter))
- Helm Charts Center (e.g. [helm charts](https://github.com/kubeservice-stack/kubservice-charts))

**This is NOT** a list of specific code locations,
  or projects. For those refer to [SIG Subprojects][sig-subprojects].

#### Cross-cutting and Externally Facing Processes

None

### Out of scope

- schduling management 

## Roles and Organization Management

This sig adheres to the Roles and Organization Management outlined in [sig-governance]
and opts-in to updates and modifications to [sig-governance].

### Additional responsibilities of Chairs

- Technical leads seeded by legacy SIG chairs from existing subproject owners

### Additional responsibilities of Tech Leads

None

### Deviations from [sig-governance]

None

### Subproject Creation

SIG Technical Leads


[readme]: https://github.com/kubeservice-stack/Community/blob/main/sig-observability
[sig-governance]: https://github.com/kubernetes/community/blob/master/committee-steering/governance/sig-governance.md
[sig-subprojects]: https://github.com/kubernetes/community/blob/master/sig-scheduling/README.md#subprojects
[Kubernetes Charter README]: https://github.com/kubernetes/community/blob/master/committee-steering/governance/README.md