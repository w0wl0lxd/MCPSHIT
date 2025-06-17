# Docker Containers Resource List

This is a comprehensive list of Docker containers currently available on the system, organized by category and purpose.

## Container Summary

**Total Containers**: 69 containers
**Currently Running**: 65 containers
**Stopped/Exited**: 4 containers

## MCP (Model Context Protocol) Servers

### Official MCP Server Containers

- **MCP Wikipedia**
  - Container: `mcp_wikipedia_mcp`
  - Image: `mcp/wikipedia-mcp:latest`
  - Status: Running
  - Purpose: Wikipedia content access via MCP

- **MCP Context7**
  - Container: `mcp_context7`
  - Image: `mcp/context7:latest`
  - Status: Running
  - Purpose: Library documentation access

- **MCP Node Code Sandbox**
  - Container: `mcp_node_code_sandbox`
  - Image: `mcp/node-code-sandbox:latest`
  - Status: Running
  - Purpose: Code execution environment

- **MCP GitHub Chat**
  - Container: `mcp_github_chat`
  - Image: `mcp/github-chat:latest`
  - Status: Running
  - Purpose: GitHub integration and chat

- **MCP JetBrains**
  - Container: `mcp_jetbrains`
  - Image: `mcp/jetbrains:latest`
  - Status: Running
  - Purpose: JetBrains IDE integration

### Custom MCP Server Containers

- **MCP Redis Server**
  - Container: `mcp-redis-server`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Redis database MCP server

- **MCP PostgreSQL Server**
  - Container: `mcp-postgres-server`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: PostgreSQL database MCP server

- **MCP GitHub**
  - Container: `mcp-github`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: GitHub API integration

- **MCP Fetch**
  - Container: `mcp-fetch`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: HTTP fetch operations

- **MCP Memory**
  - Container: `mcp-memory`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Memory management and storage

- **MCP Exa**
  - Container: `mcp-exa`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Exa search API integration

- **MCP Shodan**
  - Container: `mcp-shodan`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Shodan cybersecurity API

- **MCP ShadCN UI**
  - Container: `mcp-shadcn-ui`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: ShadCN UI component library

- **MCP Docker**
  - Container: `mcp-docker`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Docker management and operations

- **MCP Time**
  - Container: `mcp-time`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Time and date operations

- **MCP Wikipedia Server**
  - Container: `mcp-wikipedia`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Wikipedia content access

- **MCP Playwright**
  - Container: `mcp-playwright`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Browser automation and testing

- **MCP Compass**
  - Container: `mcp-compass`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: MCP server discovery

- **MCP DuckDuckGo Search**
  - Container: `mcp-ddg-search`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: DuckDuckGo search integration

- **MCP Git**
  - Container: `mcp-git`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Git repository operations

- **MCP SQLite**
  - Container: `mcp-sqlite`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: SQLite database operations

- **MCP Memory Bank**
  - Container: `mcp-memory-bank`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Persistent memory storage

- **MCP Filesystem**
  - Container: `mcp-filesystem`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: File system operations

- **MCP Brave Search**
  - Container: `mcp-brave-search`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Brave search engine integration

- **MCP Perplexica**
  - Container: `mcp-perplexica-fixed`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: Perplexica AI search

- **MCP SearXNG**
  - Container: `mcp-searxng-fixed`
  - Image: `node:20-alpine`
  - Status: Running (healthy)
  - Purpose: SearXNG meta-search engine

## Database Systems

### SQL Databases

- **PostgreSQL (Main)**
  - Container: `postgres`
  - Image: `postgres:15`
  - Status: Running
  - Ports: `0.0.0.0:5432->5432/tcp`
  - Purpose: Primary PostgreSQL database

- **PostgreSQL (MCP)**
  - Container: `thorne-mcp-postgres`
  - Image: `postgres:15`
  - Status: Running (healthy)
  - Ports: `0.0.0.0:15432->5432/tcp`
  - Purpose: PostgreSQL for MCP operations

### NoSQL Databases

- **Redis (Main)**
  - Container: `redis`
  - Image: `redis:8.0`
  - Status: Running
  - Ports: `0.0.0.0:6379->6379/tcp`
  - Purpose: Primary Redis cache/database

- **Redis (MCP)**
  - Container: `thorne-mcp-redis`
  - Image: `redis:7-alpine`
  - Status: Running (healthy)
  - Ports: `0.0.0.0:15379->6379/tcp`
  - Purpose: Redis for MCP operations

- **Redis (Stopped)**
  - Container: `myredis`
  - Image: `redis`
  - Status: Exited (1)
  - Purpose: Backup Redis instance

### Vector Databases

- **Qdrant**
  - Container: `thorne-mcp-qdrant`
  - Image: `qdrant/qdrant`
  - Status: Running
  - Ports: `0.0.0.0:6333-6334->6333-6334/tcp`
  - Purpose: Vector database for AI applications

### Search Engines

- **Meilisearch**
  - Container: `meilisearch`
  - Image: `getmeili/meilisearch:latest`
  - Status: Running
  - Purpose: Full-text search engine

## AI & Machine Learning

### Language Models

- **LocalAI**
  - Container: `local-ai`
  - Image: `localai/localai:latest-gpu-nvidia-cuda-12-extras`
  - Status: Running (healthy)
  - Ports: `0.0.0.0:8080->8080/tcp`
  - Purpose: Local AI model inference

- **Llama 3.1 8B**
  - Container: N/A (Image only)
  - Image: `ghcr.io/sozercan/llama3.1:8b`
  - Purpose: Llama 3.1 8B parameter model

### AI Development Tools

- **AnythingLLM**
  - Container: N/A (Image only)
  - Image: `mintplexlabs/anythingllm:latest`
  - Purpose: LLM management platform

- **Jupyter SciPy Notebook**
  - Container: N/A (Image only)
  - Image: `jupyter/scipy-notebook:lab-4.0.7`
  - Purpose: Data science and ML development

## Monitoring & Observability

### Metrics & Monitoring

- **Prometheus**
  - Container: `mcp-prometheus`
  - Image: `prom/prometheus:latest`
  - Status: Running
  - Ports: `0.0.0.0:9090->9090/tcp`
  - Purpose: Metrics collection and monitoring

- **Grafana**
  - Container: `thorne-mcp-grafana`
  - Image: `grafana/grafana:latest`
  - Status: Running (healthy)
  - Ports: `0.0.0.0:3001->3000/tcp`
  - Purpose: Metrics visualization and dashboards

- **Node Exporter**
  - Container: N/A (Image only)
  - Image: `prom/node-exporter:latest`
  - Purpose: System metrics collection

### Tracing & Logging

- **Jaeger**
  - Container: N/A (Image only)
  - Image: `jaegertracing/all-in-one:latest`
  - Purpose: Distributed tracing

- **OpenTelemetry Collector**
  - Container: N/A (Image only)
  - Image: `otel/opentelemetry-collector-contrib:latest`
  - Purpose: Telemetry data collection

### Application Performance

- **Pyroscope**
  - Container: N/A (Image only)
  - Image: `pyroscope/pyroscope:latest`
  - Purpose: Continuous profiling

## Docker Desktop Extensions

### Development Tools

- **Portainer Extension**
  - Container: `portainer_portainer-docker-extension-desktop-extension-service`
  - Image: `portainer/portainer-docker-extension:2.27.6`
  - Status: Running
  - Ports: `127.0.0.1:49000->9000/tcp, 127.0.0.1:49443->9443/tcp`
  - Purpose: Docker container management

- **VS Code Installer Extension**
  - Container: `docker_labs-vscode-installer-desktop-extension-service`
  - Image: `docker/labs-vscode-installer:0.0.9`
  - Status: Running
  - Purpose: VS Code installation and setup

- **AI Tools for Devs Extension**
  - Container: `docker_labs-ai-tools-for-devs-desktop-extension-service`
  - Image: `mcp/docker:0.0.17`
  - Status: Running
  - Ports: `0.0.0.0:8811->8811/tcp`
  - Purpose: AI development tools

### Security Tools

- **Copacetic Extension**
  - Container: `projectcopacetic_copacetic-docker-desktop-extension-desktop-extension-service`
  - Image: `projectcopacetic/copacetic-docker-desktop-extension:1.0.2`
  - Status: Running
  - Purpose: Container patching and security

- **Snyk Extension**
  - Container: N/A (Image only)
  - Image: `snyk/snyk-docker-desktop-extension:0.9.1`
  - Purpose: Security vulnerability scanning

- **Trivy Extension**
  - Container: N/A (Image only)
  - Image: `aquasec/trivy-docker-extension:0.4.7`
  - Purpose: Container security scanning

### Monitoring Extensions

- **Grafana Extension**
  - Container: `grafana_docker-desktop-extension-desktop-extension-grafana-docker-desktop-extension-1`
  - Image: `grafana/docker-desktop-extension:2.0.0`
  - Status: Running
  - Purpose: Grafana integration

- **Grafana Alloy**
  - Container: `grafana-docker-desktop-extension-alloy`
  - Image: `grafana/alloy:v1.0.0`
  - Status: Restarting
  - Purpose: Telemetry collection

### Utility Extensions

- **Image Tools Extension**
  - Container: `dixtdf_image-tools-desktop-extension-service`
  - Image: `dixtdf/image-tools:1.0.2`
  - Status: Running
  - Purpose: Docker image management tools

- **Rancher Application Collection**
  - Container: `rancher_application-collection-extension-desktop-extension-service`
  - Image: `rancher/application-collection-extension:0.2.2`
  - Status: Running
  - Purpose: Application deployment and management

## SignalOne AI Platform

- **SignalOne Frontend**
  - Container: `signalonefrontend`
  - Image: `signaloneai/signalonefrontend:0.1.0`
  - Status: Running
  - Ports: `0.0.0.0:37001->37001/tcp`
  - Purpose: SignalOne AI frontend interface

- **SignalOne Agent**
  - Container: `signaloneagent`
  - Image: `signaloneai/signalone-extension:0.1.0`
  - Status: Running
  - Ports: `0.0.0.0:37002->37002/tcp`
  - Purpose: SignalOne AI agent service

## Development Tools

### Version Control

- **Git (Alpine)**
  - Container: `eloquent_babbage`
  - Image: `alpine/git:latest`
  - Status: Exited (0)
  - Purpose: Git operations in Alpine Linux

### Build Tools

- **Docker Images**
  - Various containers with `docker` images
  - Purpose: Docker-in-Docker operations

- **Terraform**
  - Container: N/A (Image only)
  - Image: `hashicorp/terraform:latest`
  - Purpose: Infrastructure as Code

### Testing Tools

- **Selenium Chrome**
  - Container: N/A (Image only)
  - Image: `selenium/standalone-chrome:latest`
  - Purpose: Browser automation and testing

- **SonarQube**
  - Container: N/A (Image only)
  - Image: `sonarqube:community`
  - Purpose: Code quality analysis

## Utility Containers

### System Tools

- **File Watcher**
  - Container: `nice_kepler`
  - Image: `vonwig/inotifywait:latest`
  - Status: Running
  - Purpose: File system monitoring

- **Curl Alpine**
  - Container: N/A (Image only)
  - Image: `alpine/curl:latest`
  - Purpose: HTTP requests and testing

- **BusyBox**
  - Container: N/A (Image only)
  - Image: `busybox:latest`
  - Purpose: Minimal Unix utilities

### Networking

- **Nginx Alpine**
  - Container: N/A (Image only)
  - Image: `nginx:alpine`
  - Purpose: Web server and reverse proxy

- **Socat Alpine**
  - Container: N/A (Image only)
  - Image: `alpine/socat:latest`
  - Purpose: Network debugging and tunneling

## Temporary/Unnamed Containers

Several containers are running with temporary names and unknown specific purposes:

### Unknown Purpose Containers

- **focused_ishizaka** - Image: `93011248e2d2` (Running)
- **bold_hawking** - Image: `2aa033e58fe9` (Running)
- **musing_kepler** - Image: `f3700db496e3` (Running)
- **optimistic_khayyam** - Image: `mcp/notion:latest` (Running)
- **sharp_yonath** - Image: `93011248e2d2` (Running)
- **boring_vaughan** - Image: `f3700db496e3` (Running)
- **zealous_visvesvaraya** - Image: `2aa033e58fe9` (Running)
- **keen_greider** - Image: `2aa033e58fe9` (Running)
- **zealous_boyd** - Image: `93011248e2d2` (Running)
- **jolly_merkle** - Image: `f3700db496e3` (Running)
- **upbeat_ptolemy** - Image: `93011248e2d2` (Running)
- **busy_boyd** - Image: `2aa033e58fe9` (Running)
- **trusting_lalande** - Image: `f3700db496e3` (Running)
- **frosty_cannon** - Image: `93011248e2d2` (Running)
- **naughty_goodall** - Image: `f3700db496e3` (Running)
- **infallible_perlman** - Image: `2aa033e58fe9` (Running)
- **silly_khorana** - Image: `93011248e2d2` (Running)
- **mystifying_pike** - Image: `f3700db496e3` (Running)
- **happy_knuth** - Image: `2aa033e58fe9` (Running)
- **epic_lehmann** - Image: `93011248e2d2` (Running)
- **strange_chatelet** - Image: `f3700db496e3` (Running)
- **zen_curie** - Image: `2aa033e58fe9` (Running)

### Image ID Mapping

Based on the image listings, these containers appear to be running:
- **93011248e2d2**: `mcp/node-code-sandbox` containers
- **2aa033e58fe9**: `mcp/duckduckgo` containers  
- **f3700db496e3**: `mcp/github-chat` containers

## Container Categories Summary

- **MCP Servers**: 25 containers
- **Database Systems**: 5 containers
- **AI & Machine Learning**: 2 containers
- **Monitoring & Observability**: 2 containers
- **Docker Desktop Extensions**: 8 containers
- **SignalOne AI Platform**: 2 containers
- **Development Tools**: 3 containers
- **Utility Containers**: 3 containers
- **Unknown/Temporary**: 22 containers

## Quick Commands

### Start All MCP Servers
```bash
docker start mcp-redis-server mcp-postgres-server mcp-github mcp-fetch mcp-memory mcp-exa mcp-shodan mcp-shadcn-ui mcp-docker mcp-time mcp-wikipedia mcp-playwright mcp-compass mcp-ddg-search mcp-git mcp-sqlite mcp-memory-bank mcp-filesystem mcp-brave-search
```

### Stop All MCP Servers
```bash
docker stop mcp-redis-server mcp-postgres-server mcp-github mcp-fetch mcp-memory mcp-exa mcp-shodan mcp-shadcn-ui mcp-docker mcp-time mcp-wikipedia mcp-playwright mcp-compass mcp-ddg-search mcp-git mcp-sqlite mcp-memory-bank mcp-filesystem mcp-brave-search
```

### View All Container Status
```bash
docker ps -a --format "table {{.Names}}\t{{.Image}}\t{{.Status}}\t{{.Ports}}"
```

### Health Check All Containers
```bash
docker ps --filter "health=healthy" --format "table {{.Names}}\t{{.Status}}"
```

## Port Mappings Summary

- **Redis**: 6379 (main), 15379 (MCP)
- **PostgreSQL**: 5432 (main), 15432 (MCP)
- **Qdrant**: 6333-6334
- **LocalAI**: 8080
- **Prometheus**: 9090
- **Grafana**: 3001
- **SignalOne Frontend**: 37001
- **SignalOne Agent**: 37002
- **Portainer**: 49000, 49443
- **AI Tools Extension**: 8811
