# IoT Device Pipeline (Go Edition)

A production-grade backend microservices pipeline built using Go and AWS, designed for ingesting, processing, storing, and alerting on IoT telemetry data.

## 🎯 Goals

- Master backend microservices architecture in Go.
- Gain practical experience with core AWS services.
- Ensure robust security, observability, testing, and automated deployment.

## 🛠️ Tech Stack & AWS Services

### Backend (Go)
- **Language:** Go 1.24
- **Web Framework:** Gin or Echo
- **Databases:** PostgreSQL 17, Redis
- **Background Jobs:** River
- **Concurrency:** Goroutines & Channels
- **Observability:** OpenTelemetry, Prometheus
- **API Definition:** Protocol Buffers, OpenAPI

### AWS Integration
- **Compute & Containers:** Lambda, ECS (Fargate), Kubernetes (optional)
- **Messaging:** SNS, SQS, Kinesis
- **Databases & Storage:** DynamoDB, Timestream, S3
- **Networking & Security:** IAM, VPC, ACM, Route 53, WAF, Secrets Manager
- **Infrastructure as Code:** AWS CDK, Terraform
- **CI/CD:** GitHub Actions, AWS CodePipeline & CodeBuild
- **Monitoring:** CloudWatch, X-Ray, Grafana dashboards

## 📁 Project Structure

```
├── backends/
│   ├── device-registry      # User/device authentication
│   ├── ingestion-service    # Data ingestion endpoints
│   ├── stream-processor     # Real-time data processing
│   ├── storage-service      # Time-series data storage
│   └── alerting-service     # Notifications and alerts
│
├── libs/
│   └── api-contracts        # Shared API schemas (protobuf/OpenAPI)
│
└── deploy/
    ├── cdk                  # AWS CDK definitions
    └── terraform            # Terraform scripts (optional)
```

## 🚧 Local Development

- Easy setup using Docker Compose.
- Hot reload via [Air](https://github.com/cosmtrek/air).

## 🚀 Deployment

Automated infrastructure deployment using AWS CDK or Terraform, integrated with CI/CD pipelines via GitHub Actions or AWS CodePipeline.

## ✅ Testing

- **Unit:** Testify
- **Integration:** Docker Compose setups
- **E2E:** Postman/Newman or custom scripts

## 🔐 Security & Observability

- IAM policies, JWT authentication, RBAC
- AWS Secrets Manager
- Structured logging, tracing (OpenTelemetry/X-Ray), metrics collection

## 📌 Contribution & Roadmap

See issues for roadmap and contribution guidelines.

---

**Happy Coding! 🚀**
