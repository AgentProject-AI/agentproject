content = """# Agentic AI Security: Comparing Containers, WASM, and Kernel-Level Sandboxing

In the era of **Agentic Engineering**, the primary security bottleneck is no longer the LLM’s output, but the **Agent’s execution environment**. When an agent transitions from "thinking" to "doing"—executing code, calling APIs, or manipulating file systems—it requires a secure, isolated perimeter.

This technical deep-dive analyzes the three competing isolation paradigms: **Containers (NemoClaw)**, **WASM (IronClaw)**, and **Kernel-Level Isolation (nono)**, and how to monitor them for enterprise governance.

---

## 1. The Architecture of Isolation

The following diagram illustrates the hybrid routing and governance model required for production-grade AI agents.

```mermaid
graph TD
    %% Main Nodes
    User[User/Application]
    AgentRuntime[Agent Runtime]
    ToolRouter[Tool Router (Hybrid Architecture)]

    %% Sandbox Types
    subgraph Sandboxes
        Container[Container Sandbox (NemoClaw)]
        WASM[WASM Sandbox (IronClaw)]
        Kernel[Kernel Isolation (nono)]
    end

    %% Monitoring/Governance Layer
    subgraph Governance
        eBPF[eBPF Tracing: sys_open, tcp_connect]
        ProxyWASI[Proxy-WASI: Intercept Capabilities]
        AuditLog[Syscall Audit Logs: auditd]
    end

    %% Storage
    WORM[WORM Vault: Governance Evidence]

    %% Flow: Execution
    User -->|Requests Action| AgentRuntime
    AgentRuntime -->|Identifies Tool Call| ToolRouter

    %% hybrid decision logic
    ToolRouter -->|1. Local & GPU Required| Container
    ToolRouter -->|2. High-Frequency Logic| WASM
    ToolRouter -->|3. Sensitive/Regulated| Kernel

    %% Flow: Observation
    eBPF -.->|Observes| Container
    ProxyWASI -.->|Intercepts| WASM
    AuditLog -.->|Captures| Kernel

    %% Flow: Log Delivery
    eBPF -->|Unforgeable Evidence| WORM
    ProxyWASI -->|Intent Audit| WORM
    AuditLog -->|Provable Compliance| WORM

    %% Feedback loop
    WORM -.->|Accountability| User

    %% Styling
    style Sandboxes fill:#f0f0f0,stroke:#333,stroke-width:2px
    style Governance fill:#e1f5fe,stroke:#01579b,stroke-width:1px
    style WORM fill:#fff9c4,stroke:#fbc02d,stroke-width:2px,stroke-dasharray: 5 5
    style ToolRouter fill:#e8f5e9,stroke:#2e7d32,stroke-width:2px
