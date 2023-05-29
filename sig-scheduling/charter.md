# SIG Scheduling Charter

This charter adheres to the conventions described in the [Kubernetes Charter README] and uses
the Roles and Organization Management outlined in [sig-governance].

## Scope

SIG Scheduling is responsible for the components that make Pod placement decisions.
We build Kubernetes schedulers and scheduling features for Pods. We design and
implement features that allows users to customize placement of Pods on the nodes
of a cluster. These features include those that improve reliability of workloads,
more efficient use of cluster resources, and/or enforces placement policies. 

### In scope

SIG [readme]

#### Code, Binaries and Services

- Scheduling related features (e.g. [Namespace Node Affinity](https://github.com/kubeservice-stack/namespace-node-affinity))
- Pod scheduling Qos policies (e.g. [Custom LimitRange](https://github.com/kubeservice-stack/custom-limit-range))
- Kube-scheduler performance and scalability (e.g. [Crane Scheduler Plus](https://github.com/kubeservice-stack/crane-scheduler))
- Kube-scheduler reliability (problem detection and remediation)
- Pod scheduling APIs metrics (with [sig-observability](../sig-observability))
- Node resource management (with [Node Metric](https://github.com/kubeservice-stack/node-metrics))
- Cluster resource management (with [Node Metric](https://github.com/kubeservice-stack/node-metrics))

**This is NOT** a list of specific code locations,
  or projects. For those refer to [SIG Subprojects][sig-subprojects].

#### Cross-cutting and Externally Facing Processes

- Kube-scheduler [test grid] and [perf dashboard]

### Out of scope

- network management 
- persistent storage management

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


[test grid]: https://k8s-testgrid.appspot.com/sig-scheduling#Summary
[perf dashboard]: http://perf-dash.k8s.io/
[readme]: https://github.com/kubeservice-stack/Community/blob/main/sig-scheduling
[sig-governance]: https://github.com/kubernetes/community/blob/master/committee-steering/governance/sig-governance.md
[sig-subprojects]: https://github.com/kubernetes/community/blob/master/sig-scheduling/README.md#subprojects
[Kubernetes Charter README]: https://github.com/kubernetes/community/blob/master/committee-steering/governance/README.md