# 🚀 14-Day Curriculum — KCNA (Kubernetes and Cloud Native Associate)

> **NOTE**
> **Target Certification:** Kubernetes and Cloud Native Associate (KCNA)
> **Daily Commitment:** ~3 hours every day, including weekends
> **Progress:** Master Outline Drafted · Days 1–14 pending

This repository contains everything required to build a solid mental model of the Cloud Native ecosystem and pass the KCNA exam. It maps directly to the official CNCF syllabus, blending theory with hands-on kubectl muscle memory.

---

## ⏱️ Daily Structure (~3 hours)

| Block | Duration | Focus |
| :--- | :--- | :--- |
| **🌅 Morning** | ~1h | **Concepts & CNCF Tools.** Explaining the mental models; new material lands here while you're fresh. |
| **💻 Midday** | ~1.5h | **Hands-on Labs.** `kubectl` commands, Minikube/Kind labs, and YAML creation. Break things and observe. |
| **🎯 Afternoon** | ~0.5h | **Drills & Review.** Self-check questions with `<details>` collapsible answers. |

> **TIP**
> **Standard Topic Flow:** Context → Kubernetes Mental Model → Object Walkthrough → Hands-on YAML/CLI Exercises → Self-check questions.

---

## 🗓️ Week 1 — Kubernetes Fundamentals & Orchestration

| Day | Topic | KCNA Domain | Hands-on Focus |
| :--- | :--- | :--- | :--- |
| 1 | [K8s Architecture & Components](14-days/day-01-k8s-architecture.md) | K8s Fundamentals (46%) | `minikube start`, `kubectl cluster-info`, viewing core pods |
| 2 | [Pods, Namespaces & Isolation](14-days/day-02-pods-namespaces.md) | K8s Fundamentals | `kubectl run`, YAML structures, `kubectl logs` |
| 3 | [Controllers & Scaling](14-days/day-03-controllers-scaling.md) | K8s Fundamentals | Deployments, ReplicaSets, Rolling Updates, Rollbacks |
| 4 | [Networking Basics & Ingress](14-days/day-04-networking-services.md) | K8s Fundamentals | ClusterIP, NodePort, Port-forwarding, simple Ingress |
| 5 | [Storage & Configuration](14-days/day-05-storage-config.md) | K8s Fundamentals | Mounting PVs/PVCs, injecting ConfigMaps & Secrets |
| 6 | [Scheduling, RBAC & Security](14-days/day-06-scheduling-rbac.md) | K8s Fundamentals | Labels, Taints/Tolerations, testing RoleBindings |
| 7 | [Runtimes & Container Orchestration](14-days/day-07-runtimes-orchestration.md) | Container Orchestration (22%) | Docker vs containerd, CRI, OCI standards, `crictl` |

## 🗓️ Week 2 — Cloud Native Architecture, Delivery & Observability

| Day | Topic | KCNA Domain | Hands-on Focus |
| :--- | :--- | :--- | :--- |
| 8 | [Cloud Native Arch & CNCF Landscape](14-days/day-08-cn-architecture-landscape.md) | CN Architecture (16%) | Navigating interactive landscape, identifying core tools |
| 9 | [Service Mesh & Networking (CNI)](14-days/day-09-cni-service-mesh.md) | Container Orchestration | Calico basics, exploring the Envoy/Istio mental model |
| 10 | [App Delivery I: CI/CD Pipelines](14-days/day-10-cicd-pipelines.md) | CN App Delivery (8%) | Writing a basic GitHub Actions workflow |
| 11 | [App Delivery II: GitOps & IaC](14-days/day-11-gitops-iac.md) | CN App Delivery | ArgoCD/Flux mental model, declarative infrastructure |
| 12 | [Observability I: Telemetry & Prometheus](14-days/day-12-prometheus-metrics.md) | CN Observability (8%) | Querying basic metrics with PromQL |
| 13 | [Observability II: Logs, Traces & Cost](14-days/day-13-logs-traces-finops.md) | CN Observability | Fluentd, Jaeger, OpenTelemetry, FinOps concepts |
| 14 | [Light Review & Mock Exam](14-days/day-14-light-review.md) | All Domains | Full 60-question drill, no new material |

---

## 📂 Repository Layout

.
├── README.md                # this file
├── LICENSE
└── 14-days/
    ├── day-01-k8s-architecture.md
    ├── day-02-pods-namespaces.md
    ├── day-03-controllers-scaling.md
    ├── day-04-networking-services.md
    ├── day-05-storage-config.md
    ├── day-06-scheduling-rbac.md
    ├── day-07-runtimes-orchestration.md
    ├── day-08-cn-architecture-landscape.md
    ├── day-09-cni-service-mesh.md
    ├── day-10-cicd-pipelines.md
    ├── day-11-gitops-iac.md
    ├── day-12-prometheus-metrics.md
    ├── day-13-logs-traces-finops.md
    └── day-14-light-review.md

---

## 📚 Exam Focus — The CNCF Weighting

By Day 14 you will have built a solid foundation across all CNCF pillars. 

> **WARNING**
> **The KCNA is heavily weighted towards foundational Kubernetes concepts.**
> While the broader Cloud Native ecosystem is important, prioritize mastering the core APIs.
> 
> * **K8s Fundamentals (46%):** You must know Pods, Deployments, Services, and core architecture perfectly.
> * **Container Orchestration (22%):** Understand what Kubernetes *is*, what runtimes do (containerd), and basic security.
> * **Other Domains (32% combined):** Focus heavily on the *definitions* and *use cases* of tools (e.g., knowing ArgoCD is for GitOps, Prometheus is for metrics, Jaeger is for tracing).

---

## ✅ Pre-Exam Checklist (Day 14 Review)

- [ ] Control Plane vs. Worker Node components fully memorized (etcd, kubelet, scheduler, etc.).
- [ ] Pod lifecycle and container states understood.
- [ ] Differences between ClusterIP, NodePort, and LoadBalancer clearly defined.
- [ ] CNCF project maturity levels understood (Sandbox, Incubating, Graduated).
- [ ] The difference between an OCI image and a CRI runtime.
- [ ] Declarative vs. Imperative management (kubectl apply vs kubectl create).
- [ ] The "Three Pillars of Observability" (Metrics, Logs, Traces) mapped to CNCF tools.
- [ ] GitOps principles (single source of truth, automated reconciliation) memorized.
- [ ] Serverless vs. Microservices architecture trade-offs understood.
