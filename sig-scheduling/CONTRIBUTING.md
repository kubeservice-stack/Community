# Contributing to SIG Scheduling

Welcome to contributing to SIG Scheduling. We are excited about the prospect of you
joining our [community](https://github.com/kubeservice-stack/Community/blob/main/sig-scheduling)!

SIG Scheduling is responsible for the components that make Pod placement decisions.
You can read the SIG mission outlined in the [charter](https://github.com/kubeservice-stack/Community/blob/main/sig-scheduling/charter.md).

There are multiple ways you can participate, including PRs, issues, documentation, new proposals,
helping to answer end-user's questions, attending meetings. All kinds of contributions are welcomed.

## Before you begin

We strongly recommend you to check out the [Kubernetes Contributor Guide](https://github.com/kubeservice-stack/Community/blob/main/CONTRIBUTING.md) first.

## Getting Started Before

* If you're a newcomer and have no idea where to start, we have a non-stale pool of issues that are
available for you:
  * [first-good-issue](https://github.com/kubernetes/kubernetes/issues?q=is%3Aissue+is%3Aopen+label%3A%22good+first+issue%22+label%3Asig%2Fscheduling+)
  * [help wanted](https://github.com/kubernetes/kubernetes/issues?q=is%3Aissue+is%3Aopen+label%3A%22help+wanted%22+label%3Asig%2Fscheduling+)

* If you want to know how kube-scheduler generally works, you can read the [scheduling-eviction](https://kubernetes.io/docs/concepts/scheduling-eviction/).

* If you want to understand the architectural details of kube-scheduler, you can refer to the [design docs](https://github.com/kubernetes/community/tree/master/contributors/devel/sig-scheduling)
  or [KEPs](https://github.com/kubernetes/enhancements/tree/master/keps/sig-scheduling).

* If you have any questions, you can find us in the Kubernetes [slack](https://app.slack.com/client/T09NY5SBT/C09TP78DV).

* If you find a bug, please open an issue under kubernetes/kubernetes with labels `/sig scheduling` and `/kind bug`,
also follow the requirements of `Bug Report`, it will help us a lot when analyzing the errors.

* If you have a feature request:
  * Open an issue under kubernetes/kubernetes with labels `/sig scheduling` and `/kind feature`, please focus on
  the user stories
  * If there's any debate on the rationalities, you can bring it to the [SIG meeting](https://github.com/kubernetes/community/tree/master/sig-scheduling#meetings).
  * If there are multiple implementation options, consider creating a doc with Pros and Cons, and gather some feedback.
  You can do this by sharing the doc with the SIG's [mailing list](https://groups.google.com/forum/#!forum/kubernetes-sig-scheduling).
  * If necessary, open an issue in kubernetes/enhancements and write a [KEP](https://github.com/kubernetes/enhancements/tree/master/keps/sig-scheduling) for it.

* If you find any out-of-date documentation, please help the community correct that by either sending a PR to
update the docs or open an issue if you are not sure about how to fix it.
  * For website documentation, you can open issues at [kubernetes/website](https://github.com/kubernetes/website).
  * For developer documentation, you can open issues at [kubernetes/community](https://github.com/kubernetes/community).

* We also maintain a list of [sub projects](https://github.com/kubernetes/community/tree/master/sig-scheduling#subprojects) here.
If you're interested, you can contribute to them as well.

## Best Practices

The community has been following some practices to help ensure maintainable and quality code:


* Leave the Reviewers assigned by the bot automatically if possible, unless there is a need
for a specific contributor's expertise.

* Critical bug fixes can be assigned to approvers directly.

* Always add a new commit to address review comments instead of amending. This helps to
review the new changes. You might be asked by the Reviewer to squash at a certain point.

* Squash the commits when the PR is ready to merge, this does a great favor for the git history.

* Code contributions should be relatively small, simple, well documented and well tested.
Try to split your changes into incremental PRs if the feature is big.

* Whatever discussed offline or at the community meeting should be recorded back
to the issue/PR, which helps to preserve the context.

* Always open an issue for a TODO or a follow-up just in case you forget it.

## Use of @mentions

* @kubeservice-stack/sig-scheduling-api-reviews - API Changes and Reviews
* @kubeservice-stack/sig-scheduling-bugs - Bug Triage and Troubleshooting
* @kubeservice-stack/sig-scheduling-feature-requests - Feature Requests
* @kubeservice-stack/sig-scheduling-misc - General Discussion from Approvers and Reviewers
* @kubeservice-stack/sig-scheduling-pr-reviews - PR Reviews
* @kubeservice-stack/sig-scheduling-proposals - Design Proposals
* @kubeservice-stack/sig-scheduling-test-failures - Test Failures and Triage