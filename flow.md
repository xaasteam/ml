graph TD
    A[GitHub Repository] -->|Webhook| B[CI/CD Pipeline]
    C[OpenSearch] -->|New Data Ingestion| D[Data Processing]
    D -->|Webhook| B
    B --> E[Build and Test]
    E --> F[Train/Retrain AI Model]
    F --> G[Deploy Model]
    B --> H[Build React Client]
    B --> I[Terraform Cloud]
    I --> J[AWS Infrastructure Provisioning]
    G --> K[Deploy to AWS]
    H --> K
    K --> L[End-to-End Testing]
    L --> M[Production Deployment]