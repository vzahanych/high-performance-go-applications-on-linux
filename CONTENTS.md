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
│   │   ├── 13-scheduler.md              # GMP model, work stealing, preemption
│   │   ├── 14-memory-allocator.md       # mcache, mcentral, mheap, size classes
│   │   ├── 15-gc.md                     # Mark-sweep, GreenTeaGC experimental
│   │   ├── 16-netpoller.md              # epoll, I/O multiplexing, async I/O
│   │   ├── 17-channels.md               # Channel internals, select, patterns
│   │   ├── 18-maps.md                   # Hash tables, SwissMap (Go 1.25)
│   │   ├── 19-defer-panic-recover.md    # Stack unwinding, error handling
│   │   └── 20-profiling.md              # pprof, trace, flame graphs
│   ├── part3-observability/
│   │   ├── 21-prometheus-setup.md
│   │   ├── 22-grafana-dashboards.md
│   │   ├── 23-tracing-otlp.md
│   │   ├── 24-exporters.md              # node_exporter, cAdvisor, kube-state-metrics
│   │   ├── 25-host-vm-container.md      # Dashboards for each layer
│   │   └── 26-alerts-slos.md
│   ├── part4-s3-cache/
│   │   ├── 27-architecture.md
│   │   ├── 28-implementation.md
│   │   ├── 29-observability.md          # Wiring metrics/traces into the app
│   │   ├── 30-optimization.md
│   │   ├── 31-testing.md
│   │   ├── 32-deployment.md             # Bare metal, Docker, K8s manifests
│   │   ├── 33-troubleshooting.md
│   │   └── 34-advanced.md
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