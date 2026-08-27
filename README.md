# Yauhen Bichel

### Software Engineer · Individual Contributor · Co-Founder, MoleCare
**London, England, United Kingdom**

Software engineer with **14+ years** building **agentic AI applications, machine learning systems, big data pipelines, distributed backends and cloud infrastructure**. I build systems from scratch — from CNN model training and TensorFlow serving, through Kafka event pipelines and Spark/HDFS batch computation, to the Terraform that provisions all of it.

Polyglot backend: **Java, Go, Python, Node.js, C#/.NET**. Multi-cloud: **AWS, GCP, Azure**.

---

## 🤖 Currently building — AI SRE agents at OpenSRE

Core open-source contributor to **[OpenSRE](https://github.com/tracer-Cloud/opensre)** (Tracer's Apache-2.0 Python framework for **AI Site Reliability Engineering agents**, 10k+ ★).

- **Benchmarking & evaluation environment for LLM agents** — AWS environment provisioned with Terraform, PR-time CI (tflint, tfsec, checkov), a Dockerized bench container pushed to ECR, an S3-backed dataset pipeline, and provenance capture for benchmark reports
- **Large-scale architecture restructuring** into a `core / surfaces / integrations / tools` layout — broke 7+ import cycles with a **Tarjan strongly-connected-components cycle scanner** plus a CI guard enforcing import direction
- **Unified LLM provider routing** into a single provider factory with a typed client interface and adapter registry; decomposed the `Session` god object and the agent harness into cohesive, testable packages
- **OpenTelemetry-style session-trace span port** capturing per-stage, per-tool and per-LLM metrics
- **Lazy, surface-scoped tool registry** backed by a static descriptor index over 60+ integrations, cutting agent startup cost

`Python` `LLM agents` `AI SRE` `AWS` `Terraform` `Docker` `OpenTelemetry` `pytest` `GitHub Actions`

---

## 🧠 Machine Learning, Deep Neural Networks & AI

- **CNN melanoma prediction** — trained convolutional neural networks for skin-lesion classification at MoleCare; published as *[Melanoma Prediction Using CNN Methods](https://medium.com/@yauhen.bichel)*
- **Production ML serving pipeline** — REST API → **Kafka** → **TensorFlow Serving**, with models trained on **GCP Vertex AI**
- **Face recognition with neural networks** — [comparative study of NN algorithms](https://github.com/YauhenBichel/Face-Recognition-Using-Neural-Networks-My-graduate-Project) for facial recognition (graduate project, C#)
- **Deep neural network research** — [My Study of Deep Neural Networks](https://github.com/YauhenBichel/My-Study-of-Deep-Neural-Networks)
- **Reinforcement learning for AI SRE** — [tracer-sre-rl](https://github.com/YauhenBichel/tracer-sre-rl)
- **MLOps** — [MLflow, Metaflow and Weights & Biases pipelines](https://github.com/YauhenBichel/my-experiments-with-mlops-zoomcamp) (Research Assistant, University of San Francisco)
- **Agentic apps & MCP** — [AI App with MCP Servers](https://github.com/YauhenBichel/AI-App-with-MCP-Servers), DALL·E and Replicate APIs

*Certified: Neural Networks and Deep Learning · Improving Deep Neural Networks: Hyperparameter Tuning, Regularization and Optimization (deeplearning.ai)*

---

## 📊 Big Data & Distributed Computation

- **Team Leader / Big Data Engineer at Nielsen** — led development of a REST API processing data via **Apache Spark on HDFS** with Cloudera and Zookeeper, Docker deployments on Kubernetes, Jenkins CI/CD with Checkmarx security scanning
- **S3-backed dataset pipeline** for AI-agent benchmark corpora at OpenSRE
- Data stores across the stack: **PostgreSQL, MySQL, MongoDB, MS SQL Server, Redis**

`Spark` `HDFS` `Cloudera` `Zookeeper` `Kafka` `ELK Stack`

---

## 🔌 APIs & Distributed Services

- [**URL Shortener**](https://github.com/YauhenBichel/URL-Shortener) — TinyURL-style service using Base62 encoding, Spring Boot, Redis and React
- [**REST API rate limiting & throttling**](https://github.com/YauhenBichel/API-REST-Limit-and-Throttling) — request-per-second control and client-side API limits
- [**Services with service mesh and gRPC**](https://github.com/YauhenBichel/Services-with-Mesh-and-gRPC)
- [**API using raw sockets and servlets**](https://github.com/YauhenBichel/API-using-sockets-and-servlets) — Jetty server, no framework
- [**Booking API**](https://github.com/YauhenBichel/Test-Project-Booking-API) (Java/Spring) · [**Go REST API**](https://github.com/YauhenBichel/go-rest-api) · [**Customers Web API**](https://github.com/YauhenBichel/Customers-Web-API) (.NET Core)
- [**Resilience4j retry patterns**](https://github.com/YauhenBichel/Retry-with-resilience4j) — circuit breaking and retry under load
- Microservices, **REST · gRPC · SOAP/RPC**, API-key authentication, JWT and Apple Sign-In, billing microservice built from scratch with Spring Integration and Spring Batch

---

## 📨 Message & Streaming Systems

- [**Kafka deployment on AWS**](https://github.com/YauhenBichel/Kafka-Deployment-using-AWS) — production Kafka for MoleCare's ML inference pipeline
- Event-driven architecture with **Kafka, Kafka Streams, RabbitMQ** and **AWS EventBridge**
- [**Multithreaded Java**](https://github.com/YauhenBichel/Multithreaded-Java-Program-Read-Files) — `ExecutorService`, `ReentrantLock`, `CountDownLatch`

*Certified: Stream Processing using Apache Kafka Streams and Confluent ksqlDB*

---

## ☁️ Cloud Infrastructure, IaC & Observability

**HashiCorp Certified: Terraform Associate (003)**

- [**tf-module-aws-batch-job-revision**](https://github.com/YauhenBichel/tf-module-aws-batch-job-revision) · [**tf-module-aws-eventbridge-batch-trigger**](https://github.com/YauhenBichel/tf-module-aws-eventbridge-batch-trigger) · [**tf-module-aws-parameter-store**](https://github.com/YauhenBichel/tf-module-aws-parameter-store) — reusable Terraform modules
- [**github-action-terraform-output**](https://github.com/YauhenBichel/github-action-terraform-output) — GitHub Actions workflow action for Terraform outputs
- [**linux-perf-tools-board**](https://github.com/YauhenBichel/linux-perf-tools-board) — Go dashboard unifying Linux performance tooling
- [**react-otel-sample**](https://github.com/YauhenBichel/react-otel-sample) — front-end OpenTelemetry instrumentation
- **OpenTelemetry observability PoC** for a multi-cloud (AWS + Azure) platform at UCL — surfaced the monitoring gaps and secured budget for implementation
- Private-cloud faculty deployments with **Rancher, Ansible, Helm, Terraform Cloud**; Go CLI for artifact management shipping to JFrog Artifactory

`AWS (Lambda, Batch, ECR, EventBridge, Aurora, SES, EC2, S3)` `GCP (Vertex AI)` `Azure` `Kubernetes` `Docker` `Helm` `Grafana` `Zipkin` `Jaeger` `Splunk`

---

## 🧮 Algorithms & Data Structures

- [**Algorithms and Data Structures in Java**](https://github.com/YauhenBichel/Algorithms-and-data-structures) — sorting, graphs, trees, dynamic programming, with complexity analysis
- [**LeetCode: /ybichel**](https://leetcode.com/ybichel/)
- [**Comparators in Java**](https://github.com/YauhenBichel/Comparators-in-java) · [**Dependency Injection from scratch**](https://github.com/YauhenBichel/Dependency-Injection) — a minimal Spring-style DI container · [**Luhn algorithm token validation**](https://github.com/YauhenBichel/Generate-tokens-and-validate-them)

---

## 🏥 MoleCare — Co-Founder & Founding Software Engineer

Healthcare application for skin lesion monitoring, **published on the NHS App Library**. I designed the full architecture: Java/Spring REST API, PostgreSQL, Kafka on AWS EC2, TensorFlow model serving, React web app and React Native mobile app — then migrated the whole platform from Heroku to AWS.

🌐 [molecare.co.uk](https://www.molecare.co.uk)

---

## 🎓 Education & Publications

**MSc Computer Science** — University of Greenwich
**Diploma in Computers, Systems and Networks** — Belarusian State University of Informatics and Radioelectronics

- *Melanoma Prediction Using CNN Methods*
- *Kafka in MoleCare using AWS*
- *MoleCare is Live on the NHS App Library*
- *Rest Less (restless.co.uk) — feature on MoleCare*

---

## 📫 Get in touch

**Open to Staff / Principal / Lead engineering roles — AI & ML platforms, data infrastructure and distributed backends. London or remote.**

[![LinkedIn](https://img.shields.io/badge/LinkedIn-yauhen--bichel-0A66C2?logo=linkedin&logoColor=white)](https://www.linkedin.com/in/yauhen-bichel)
[![Medium](https://img.shields.io/badge/Medium-@yauhen.bichel-000000?logo=medium&logoColor=white)](https://medium.com/@yauhen.bichel)
[![LeetCode](https://img.shields.io/badge/LeetCode-ybichel-FFA116?logo=leetcode&logoColor=white)](https://leetcode.com/ybichel/)
[![Email](https://img.shields.io/badge/Email-yauhen.bichel@gmail.com-EA4335?logo=gmail&logoColor=white)](mailto:yauhen.bichel@gmail.com)

<!--
Keywords for discovery: Yauhen Bichel, Staff Software Engineer London, machine learning engineer,
deep neural networks, CNN, TensorFlow, agentic AI, LLM agents, AI SRE, MLOps, Vertex AI,
big data, Apache Spark, HDFS, Kafka, event-driven architecture, REST API, gRPC, microservices,
distributed systems, Terraform, AWS, Azure, GCP, Kubernetes, OpenTelemetry, observability,
Java, Go, Golang, Python, algorithms and data structures.
-->
