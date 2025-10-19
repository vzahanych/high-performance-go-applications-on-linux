manuscript/               # Book content (Markdown)
│   ├── part1-linux/
│   │   ├── 01-memory.md
│   │   ├── 02-cpu.md
│   │   ├── 03-networking.md
│   │   ├── 04-storage.md
│   │   ├── 05-syscalls.md
│   │   ├── 06-ipc.md
│   │   ├── 07-containerization.md
│   │   ├── 08-virtualization.md
│   │   ├── 09-containers-inside-vms.md
│   │   ├── 10-kubernetes-essentials.md  # Control plane, nodes, pods, kubelet
│   │   ├── 11-kubernetes-networking.md  # CNI, Services, kube-proxy, Ingress
│   │   └── 12-kubernetes-storage.md     # PV/PVC, CSI drivers, ephemeral storage
│   ├── part2-go-runtime/
│   │   ├── 13-scheduler.md
│   │   ├── 14-gc.md
│   │   ├── 15-netpoller.md
│   │   └── 16-profiling.md
│   ├── part3-observability/
│   │   ├── 17-prometheus-setup.md
│   │   ├── 18-grafana-dashboards.md
│   │   ├── 19-tracing-otlp.md
│   │   ├── 20-exporters.md              # node_exporter, cAdvisor, kube-state-metrics
│   │   ├── 21-host-vm-container.md      # Dashboards for each layer
│   │   └── 22-alerts-slos.md
│   ├── part4-s3-cache/
│   │   ├── 23-architecture.md
│   │   ├── 24-implementation.md
│   │   ├── 25-observability.md          # Wiring metrics/traces into the app
│   │   ├── 26-optimization.md
│   │   ├── 27-testing.md
│   │   ├── 28-deployment.md             # Bare metal, Docker, K8s manifests
│   │   ├── 29-troubleshooting.md
│   │   └── 30-advanced.md
│   ├── appendices/
│   │   ├── a-quick-reference.md
│   │   ├── b-tools-setup.md
│   │   ├── c-performance-patterns.md
│   │   ├── d-production-checklist.md
│   │   └── e-further-learning.md
│   ├── frontmatter/
│   │   ├── title.md
│   │   ├── copyright.md
│   │   ├── dedication.md
│   │   ├── foreword.md
│   │   ├── preface.md
│   │   └── acknowledgments.md
│   └── metadata.yaml        # Pandoc metadata (title, 