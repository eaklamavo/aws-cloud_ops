# Infrastructure as Code Study Plan (Terraform + Docker + Kubernetes + Argo CD)

A lightweight, hands-on path to learn modern IaC and GitOps workflows from beginner to intermediate level.

## Prerequisites

- Basic terminal usage (bash)
- Git installed and configured
- Jupyter Notebook or JupyterLab
- Docker Desktop or Docker Engine
- Terraform CLI (>= 1.6)
- `kubectl`
- A Kubernetes cluster for practice (kind, minikube, or k3d)
- Optional: Argo CD installed on your practice cluster

## Recommended Resources

### 📋 Official Specification / Exam Guide
| Resource | URL |
|----------|-----|
| Terraform Language Documentation | https://developer.hashicorp.com/terraform/language |
| Terraform Release Notes | https://github.com/hashicorp/terraform/releases |
| Docker Engine Release Notes | https://docs.docker.com/engine/release-notes/ |
| Kubernetes Release Notes | https://kubernetes.io/releases/ |
| Argo CD Releases | https://github.com/argoproj/argo-cd/releases |

### 📚 Core Documentation
| Resource | URL |
|----------|-----|
| Terraform Docs | https://developer.hashicorp.com/terraform/docs |
| Terraform CLI Command Reference | https://developer.hashicorp.com/terraform/cli/commands |
| Docker Docs | https://docs.docker.com/ |
| Docker CLI Reference | https://docs.docker.com/reference/cli/docker/ |
| Kubernetes Docs | https://kubernetes.io/docs/home/ |
| kubectl Reference | https://kubernetes.io/docs/reference/kubectl/ |
| Argo CD Official Docs | https://argo-cd.readthedocs.io/en/stable/ |

### 🎓 Training & Courses
| Resource | URL |
|----------|-----|
| HashiCorp Terraform Tutorials (official) | https://developer.hashicorp.com/terraform/tutorials |
| Docker Getting Started (official) | https://docs.docker.com/get-started/ |
| Kubernetes Basics (official interactive tutorial) | https://kubernetes.io/docs/tutorials/kubernetes-basics/ |
| Argo CD Getting Started | https://argo-cd.readthedocs.io/en/stable/getting_started/ |
| CNCF YouTube (talks and walkthroughs) | https://www.youtube.com/@CloudNativeFdn |

### 📝 Cheat Sheets & Quick Reference
| Resource | URL |
|----------|-----|
| kubectl Cheat Sheet | https://kubernetes.io/docs/reference/kubectl/cheatsheet/ |
| Terraform CLI Quick Reference | https://developer.hashicorp.com/terraform/cli/commands |
| Docker CLI Reference (command quick lookup) | https://docs.docker.com/reference/cli/docker/ |
| Argo CD CLI Command Reference | https://argo-cd.readthedocs.io/en/stable/user-guide/commands/argocd/ |

### 🛠️ Key Docs by Phase/Feature
| Phase | Feature | URL |
|-------|---------|-----|
| Phase 1 | IaC fundamentals and workflow | https://developer.hashicorp.com/terraform/intro |
| Phase 1 | Docker images and containers | https://docs.docker.com/get-started/docker-concepts/the-basics/what-is-a-container/ |
| Phase 1 | Kubernetes architecture basics | https://kubernetes.io/docs/concepts/overview/components/ |
| Phase 2 | Terraform providers/resources/state | https://developer.hashicorp.com/terraform/language/state |
| Phase 2 | Terraform variables and modules | https://developer.hashicorp.com/terraform/language/modules |
| Phase 2 | Remote state and teams | https://developer.hashicorp.com/terraform/language/backend |
| Phase 3 | Kubernetes deployments/services | https://kubernetes.io/docs/concepts/workloads/controllers/deployment/ |
| Phase 3 | Argo CD application model | https://argo-cd.readthedocs.io/en/stable/core_concepts/ |
| Phase 3 | GitOps continuous delivery | https://argo-cd.readthedocs.io/en/stable/operator-manual/declarative-setup/ |

### 🧪 Practice & Sandboxes
| Resource | URL |
|----------|-----|
| Play with Docker | https://labs.play-with-docker.com/ |
| Killercoda Labs (Kubernetes, Docker, Terraform) | https://killercoda.com/ |
| kind (Kubernetes in Docker) | https://kind.sigs.k8s.io/ |
| Argo CD Example Apps | https://github.com/argoproj/argocd-example-apps |

### 🏘️ Community & Support
| Resource | URL |
|----------|-----|
| Terraform GitHub | https://github.com/hashicorp/terraform |
| Kubernetes Slack | https://slack.k8s.io/ |
| Kubernetes GitHub | https://github.com/kubernetes/kubernetes |
| Argo Project Slack | https://argoproj.github.io/community/join-slack/ |
| Argo CD GitHub | https://github.com/argoproj/argo-cd |
| Stack Overflow (terraform tag) | https://stackoverflow.com/questions/tagged/terraform |
| Stack Overflow (kubernetes tag) | https://stackoverflow.com/questions/tagged/kubernetes |

## Study Plan Overview

| Phase | Title | Lessons | Est. Time |
|-------|-------|---------|-----------|
| 1 | Foundations & Tooling | 3 | 3-4 hrs |
| 2 | Terraform IaC Core | 3 | 4-5 hrs |
| 3 | Containers, Kubernetes & Argo CD | 3 | 4-5 hrs |
| - | Capstone | 1 | 3-4 hrs |

**Total: 9 lessons + 1 capstone (~14-18 hours)**

## Lessons

### Phase 1 - Foundations & Tooling
| # | Notebook | Topic |
|---|----------|-------|
| 1.1 | [lesson-1.1-iac-mental-model.ipynb](phase-1-foundations-tooling/lesson-1.1-iac-mental-model.ipynb) | IaC mental model, declarative workflow, local setup |
| 1.2 | [lesson-1.2-docker-basics.ipynb](phase-1-foundations-tooling/lesson-1.2-docker-basics.ipynb) | Build and run a containerized app |
| 1.3 | [lesson-1.3-kubernetes-basics.ipynb](phase-1-foundations-tooling/lesson-1.3-kubernetes-basics.ipynb) | Deploy first app to Kubernetes |

### Phase 2 - Terraform IaC Core
| # | Notebook | Topic |
|---|----------|-------|
| 2.1 | [lesson-2.1-terraform-providers-state.ipynb](phase-2-terraform-iac/lesson-2.1-terraform-providers-state.ipynb) | Providers, resources, init/plan/apply |
| 2.2 | [lesson-2.2-terraform-variables-modules.ipynb](phase-2-terraform-iac/lesson-2.2-terraform-variables-modules.ipynb) | Variables, outputs, reusable modules |
| 2.3 | [lesson-2.3-terraform-remote-state-workflows.ipynb](phase-2-terraform-iac/lesson-2.3-terraform-remote-state-workflows.ipynb) | Remote state, locking, team workflow |

### Phase 3 - Containers, Kubernetes & Argo CD
| # | Notebook | Topic |
|---|----------|-------|
| 3.1 | [lesson-3.1-kubernetes-manifests-services.ipynb](phase-3-containers-kubernetes/lesson-3.1-kubernetes-manifests-services.ipynb) | Deployments, services, config updates |
| 3.2 | [lesson-3.2-argocd-gitops-basics.ipynb](phase-3-containers-kubernetes/lesson-3.2-argocd-gitops-basics.ipynb) | Argo CD app model and GitOps sync |
| 3.3 | [lesson-3.3-end-to-end-iac-gitops.ipynb](phase-3-containers-kubernetes/lesson-3.3-end-to-end-iac-gitops.ipynb) | Terraform + Kubernetes + Argo CD flow |

### Capstone
| Notebook | Description |
|----------|-------------|
| [capstone-project.ipynb](capstone/capstone-project.ipynb) | Build a small GitOps platform: infra definitions, app manifests, and Argo CD continuous reconciliation |

## Capstone Overview

Build a practical mini-platform where:

- Terraform defines baseline infrastructure and Kubernetes namespace conventions
- Docker packages a sample app image
- Kubernetes manifests define the running workload
- Argo CD continuously syncs desired state from Git

You will finish with a repeatable delivery workflow suitable for dev/staging/prod adaptation.

## How to Use the Notebooks

1. Install Jupyter: `pip install notebook` or `pip install jupyterlab`
2. Launch Jupyter from this directory
3. Open lessons in order and run cells top-to-bottom
4. Complete all `# TODO:` or `# TASK:` exercise cells
5. Keep generated files in a local `work/` folder for later lessons
