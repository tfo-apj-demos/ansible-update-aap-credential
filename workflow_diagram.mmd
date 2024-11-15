flowchart TD
    subgraph GitLab["GitLab "]
        A[CI/CD Pipeline Trigger]
        subgraph Jobs["Sequential Pipeline Jobs"]
            B[Job 1: Rotate Vault Secret ID]
            B -->|Sequential| C[Job 2: Update AAP Credential]
        end
    end
    subgraph OpenShift["OpenShift Cluster"]
        subgraph Runner["Namespace: gitlab-runner"]
            D[GitLab Runner]
        end
        subgraph AAP["Namespace: aap"]
            E[Ansible Automation Platform]
            F[Job template]
        end
    end
    subgraph Infrastructure["vSphere"]
        G[HashiCorp Vault]
    end
    A -->|Triggers| B
    B -->|Requests rotation| G
    G -->|Returns new Secret ID| B
    C -->|Updates credential in| E
    E -->|Then executes| F
    style F stroke-width:2px,stroke-dasharray: 5, 5  % thicker, dashed line
    F -.->|Configures| E
    D -->|Executes jobs sequentially| B
    style GitLab fill:#FFECEC,stroke:#FF9999
    style OpenShift fill:#E7F5FF,stroke:#7FBFFF
    style Infrastructure fill:#E8F5E9,stroke:#81C784
    style Jobs fill:#FFE5CC,stroke:#FFB366
