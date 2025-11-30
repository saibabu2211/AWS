# Table Notes

## 🏗️ AWS Well-Architected Framework (WAF)

The framework is built on **6 Pillars**:

| Pillar | Focus | Example Exam Question Style |
| --- | --- | --- |
| **1. Operational Excellence** | Run & monitor systems, improve processes | *“Which pillar focuses on monitoring and continuous improvement?”* |
| **2. Security** | Protect data, systems, and assets | *“Which pillar covers IAM, encryption, and detective controls?”* |
| **3. Reliability** | Ensure workloads perform correctly, recover quickly | *“Which pillar includes Multi-AZ deployments?”* |
| **4. Performance Efficiency** | Use IT/resources efficiently, scale on demand | *“Which pillar focuses on using the right instance type for workload?”* |
| **5. Cost Optimization** | Avoid unnecessary costs, optimize spend | *“Which pillar uses right-sizing, spot instances?”* |
| **6. Sustainability** | Minimize environmental impact of workloads | *“Which pillar focuses on reducing waste & energy efficiency?”* |
- ⚡ Exam Confusion Points
    - **Reliability vs Availability vs Fault Tolerance**
        
        👉 Reliability = system continues to function.
        
        👉 Availability = system uptime.
        
        👉 Fault Tolerance = system continues even if parts fail.
        
    - **Security Pillar vs Operational Excellence**
        
        👉 Security = *protecting data & resources*.
        
        👉 Operational = *improving operations, monitoring*.
        
    - **Performance Efficiency vs Cost Optimization**
        
        👉 Performance = best resource for job.
        
        👉 Cost = cheapest way to run job.
        
    - **Sustainability** is **new** → exam may trick you.
        
        👉 Example: *“Which pillar reduces environmental impact of workloads?”* = **Sustainability**.
        
- 🧠 3 Key Best Practice Questions They Like
    1. **Which service/tool helps measure workload against the Well-Architected Framework?**
        
        👉 *Answer = AWS Well-Architected Tool.*
        
    2. **Which pillar is about encrypting data in transit & at rest?**
        
        👉 *Answer = Security.*
        
    3. **Which pillar is about designing systems that recover quickly from failure?**
        
        👉 *Answer = Reliability.*
        

---

## 1. **Security Groups vs NACLs**

| Feature | Security Group | NACL |
| --- | --- | --- |
| Level | Instance level | Subnet level |
| Stateful / Stateless | Stateful | Stateless |
| Default behavior | Deny all inbound, allow all outbound | Allow all in/out |
| Rule type | Allow only | Allow + Deny |
| Applies to | EC2 instances | All resources in subnet |

## 2.  AWS Compute Services Comparison

| Service | Type | Key Features | Best For |
| --- | --- | --- | --- |
| **EC2 (Elastic Compute Cloud)** | Virtual servers (IaaS) | Full control over OS, networking, storage. Pay per use. | Custom apps, lift & shift workloads. |
| **Lambda** | Serverless (FaaS) | Runs code without servers, pay per execution. Event-driven. | Event-based apps, automation, microservices. |
| **Elastic Beanstalk** | Platform as a Service (PaaS) | Deploy apps (Java, Python, Node, etc.) with auto-scaling & monitoring built-in. | Developers who want to deploy fast without infra mgmt. |
| **Lightsail** | VPS (simplified compute) | Pre-configured with OS, DB, networking, load balancer. Easy UI. | Small websites, blogs, testing apps. |
| **ECS (Elastic Container Service)** | Container orchestration | AWS-managed Docker orchestration. Runs on EC2 or Fargate. | Containerized apps without needing Kubernetes. |
| **EKS (Elastic Kubernetes Service)** | Managed Kubernetes | Runs K8s clusters, integrates with AWS services. | Teams using Kubernetes. |
| **Fargate** | Serverless containers | Run ECS/EKS containers without managing servers. | Containers without EC2. |
| **Batch** | Batch processing | Run large-scale batch jobs efficiently. | Scientific computing, big data batch workloads. |
| **Outposts** | Hybrid compute | Extends AWS infra on-prem. | Low-latency on-prem + AWS integration. |

## 📦 AWS Storage Services Comparison

| Service | Type | Key Features | Best For |
| --- | --- | --- | --- |
| **S3 (Simple Storage Service)** | Object storage | Unlimited storage, 11 9’s durability, global namespace, lifecycle policies, versioning. | Backup, media, static website hosting, data lake. |
| **EBS (Elastic Block Store)** | Block storage (like hard drive) | Attached to single EC2, low-latency, must be in same AZ as EC2. | Databases, OS boot volumes, transactional workloads. |
| **EFS (Elastic File System)** | File storage (NFS) | Fully managed, shared across multiple EC2 instances, scalable. | Content management, big data, multi-server apps. |
| **FSx (File System for Windows/Lustre)** | Managed file system | FSx for Windows = SMB support, FSx for Lustre = high-performance HPC. | Windows workloads, high-performance computing. |
| **Glacier / Glacier Deep Archive** | Archival object storage | Ultra-cheap storage, retrieval time minutes–hours. | Long-term backups, compliance data, archives. |
| **Storage Gateway** | Hybrid storage | Connects on-prem apps to AWS storage (S3, Glacier, etc.). | Hybrid cloud storage, backup/restore. |
| **Snow Family (Snowcone, Snowball, Snowmobile)** | Data transfer appliances | Move TB–EB data physically to AWS. | Data migration, disconnected environments. |

## 🗄️ AWS Database Services Comparison

| Service | Type | Key Features | Best For |
| --- | --- | --- | --- |
| **RDS (Relational Database Service)** | Relational (SQL) | Managed DB (MySQL, PostgreSQL, MariaDB, Oracle, SQL Server). Handles backups, patching, Multi-AZ, read replicas. | Traditional apps needing relational DB. |
| **Aurora** | Relational (SQL, MySQL/PostgreSQL compatible) | AWS-built, 5× faster than MySQL, auto scaling, serverless option. | High-performance relational DB, modern apps. |
| **DynamoDB** | NoSQL (key-value, document) | Fully managed, serverless, single-digit ms latency, auto scaling, global tables. | Gaming, IoT, real-time apps, serverless apps. |
| **Redshift** | Data warehouse (analytical SQL) | Columnar storage, integrates with BI tools, petabyte scale. | Analytics, reporting, OLAP queries. |
| **ElastiCache (Redis/Memcached)** | In-memory cache | Super fast (microsecond latency), offload reads from DB. | Caching, session storage, gaming leaderboards. |
| **Neptune** | Graph database | Relationships between data (social, recommendation engines). | Social networks, fraud detection, knowledge graphs. |
| **DocumentDB** | Document database (MongoDB compatible) | Fully managed, JSON-like storage. | Applications using MongoDB. |
| **Keyspaces (for Apache Cassandra)** | Wide column NoSQL | Scalable, serverless Cassandra-compatible DB. | IoT, time series data, big NoSQL apps. |
| **Qldb (Quantum Ledger DB)** | Ledger DB | Immutable transaction log, cryptographically verifiable. | Supply chain, finance, audit trails. |
| **Timestream** | Time series database | Optimized for time-stamped data. | IoT telemetry, monitoring, analytics. |
- 🧠 Exam Tips (Database)
    1. If it says **“transactional system”** → RDS or Aurora.
    2. If it says **“analytics or BI”** → Redshift.
    3. If it says **“serverless NoSQL”** → DynamoDB.
    4. If it says **“caching layer”** → ElastiCache.
    5. If it says **“social network / relationships”** → Neptune.
    6. If it says **“ledger / immutable transactions”** → QLDB.
    7. If it says **“time series data”** → Timestream.
- ⚡ Quick Confusing Pairs
    - **RDS vs Aurora**
        
        👉 RDS = managed traditional DB.
        
        👉 Aurora = AWS-optimized relational DB (faster, serverless).
        
    - **RDS vs DynamoDB**
        
        👉 RDS = SQL (structured schema).
        
        👉 DynamoDB = NoSQL (key-value, unstructured).
        
    - **Redshift vs RDS**
        
        👉 Redshift = analytics/data warehouse (OLAP).
        
        👉 RDS = transactional processing (OLTP).
        
    - **ElastiCache vs DynamoDB DAX**
        
        👉 ElastiCache = standalone cache service.
        
        👉 DynamoDB DAX = caching layer specifically for DynamoDB.
        
    - **Neptune vs DocumentDB**
        
        👉 Neptune = graph DB (nodes + relationships).
        
        👉 DocumentDB = document DB (JSON).
        

---

## 🤖 AWS Machine Learning Services Comparison

| Service | Type | Key Features | Best For |
| --- | --- | --- | --- |
| **SageMaker** | Build, train, deploy ML models | End-to-end ML platform. Jupyter notebooks, AutoML, model hosting. | Data scientists, ML developers building custom ML. |
| **Rekognition** | Computer vision (image/video) | Detect faces, objects, unsafe content, celebrity recognition. | Security, media, surveillance, photo apps. |
| **Comprehend** | Natural Language Processing (NLP) | Sentiment analysis, entity recognition, topic modeling. | Customer feedback, document analysis, chatbots. |
| **Lex** | Conversational AI | Build chatbots & voice assistants (tech behind Alexa). | Customer support, voice/text chatbots. |
| **Polly** | Text-to-speech | Convert text into natural speech. | Voice apps, audiobooks, accessibility tools. |
| **Transcribe** | Speech-to-text | Automatic speech recognition (ASR). | Transcribing calls, captions, audio-to-text. |
| **Translate** | Machine translation | Language translation at scale. | Multilingual websites, apps, support. |
| **Personalize** | Recommendation engine | Similar to Amazon.com recommendations. | Product recommendations, personalization. |
| **Forecast** | Time series forecasting | Demand prediction, sales forecasting, capacity planning. | Retail, finance, supply chain. |
| **Textract** | OCR (Optical Character Recognition) | Extracts text, tables, forms from scanned docs. | Invoices, forms, document digitization. |
| **Kendra** | Intelligent search | ML-powered enterprise search engine. | Company knowledge base, document search. |
- ⚡ Quick Confusing Pairs
    - **Comprehend vs Translate**
        
        👉 Comprehend = NLP (sentiment, entities).
        
        👉 Translate = language translation.
        
        - **Polly vs Transcribe**
            
            👉 Polly = text → speech.
            
            👉 Transcribe = speech → text.
            
        - **Rekognition vs Textract**
            
            👉 Rekognition = images/videos.
            
            👉 Textract = scanned docs/forms.
            
        - **Lex vs Connect**
            
            👉 Lex = build chatbot.
            
            👉 Connect = contact center solution (can use Lex bots).
            
        - **Forecast vs Personalize**
            
            👉 Forecast = predict future demand.
            
            👉 Personalize = recommend products/content.
            
- 🧠 Exam Tips (ML)
    1. If question mentions **build/train ML models** → **SageMaker**.
    2. If **image/video analysis** → **Rekognition**.
    3. If **text sentiment / NLP** → **Comprehend**.
    4. If **chatbot** → **Lex**.
    5. If **voice to text** → **Transcribe**.
    6. If **text to voice** → **Polly**.
    7. If **translate language** → **Translate**.
    8. If **document OCR** → **Textract**.
    9. If **search knowledge base** → **Kendra**.
    10. If **recommend products** → **Personalize**.
    11. If **predict demand/time series** → **Forecast**.

---

# 🔐 AWS Security Services Comparison

| Service | Purpose | Key Features | Use Case | Confusing With |
| --- | --- | --- | --- | --- |
| **IAM (Identity & Access Management)** | Manage *who* can access AWS resources | Users, Groups, Roles, Policies, MFA | Controlling access at user/role level | Confused with Organizations or SSO |
| **AWS Organizations** | Manage multiple AWS accounts centrally | SCPs (Service Control Policies), consolidated billing | Large org with multiple accounts | Confused with IAM (since both “control access”) |
| **AWS Cognito** | Authentication for apps (sign-in/signup) | User Pools, Identity Pools, social login | Mobile/web app user auth | Confused with IAM |
| **AWS SSO (IAM Identity Center)** | Centralized login for multiple AWS accounts/apps | Connects with AD/Okta, assigns roles across accounts | Enterprise SSO for workforce | Confused with Cognito |
| **KMS (Key Management Service)** | Encrypt/decrypt data with managed keys | CMKs, envelope encryption, integrates with S3, EBS, RDS | Secure data at rest & in transit | Confused with Secrets Manager |
| **AWS Secrets Manager** | Store & rotate secrets | Auto password rotation, encrypts with KMS | DB credentials, API keys | Confused with SSM Parameter Store |
| **SSM Parameter Store** | Store configuration & secrets | Hierarchical storage, basic secrets management | App configs, environment variables | Confused with Secrets Manager |
| **Shield** | DDoS protection | Standard (free), Advanced (paid, 24/7 support) | Protects websites/apps | Confused with WAF |
| **WAF (Web Application Firewall)** | Filter/block malicious web traffic | Rules, managed rule groups, integrates with ALB, CloudFront | Block SQLi, XSS | Confused with Shield |
| **Inspector** | Automated security assessment | Scans for vulnerabilities in EC2, ECR, Lambda | Compliance & security scanning | Confused with GuardDuty |
| **GuardDuty** | Threat detection & monitoring | Analyzes VPC flow logs, DNS logs, CloudTrail events | Detect compromised accounts, malware | Confused with Inspector |
| **Macie** | Data security for S3 | ML-powered PII detection, sensitive data classification | GDPR/PCI compliance | Confused with GuardDuty |
| **CloudTrail** | Record API activity in AWS | Tracks “who did what and when” | Audit logs | Confused with CloudWatch |
| **CloudWatch** | Monitoring and alerting | Metrics, logs, alarms, dashboards | Performance & operational monitoring | Confused with CloudTrail |
- 👉 **Memory Trick**
    - **IAM = Who can access AWS**
    - **Organizations = Manage multiple accounts**
    - **Cognito = Sign-up / Sign-in for apps**
    - **SSO = One login for many AWS accounts**
    - **KMS = Encrypt data**
    - **Secrets Manager = Manage passwords**
    - **Parameter Store = App configs**
    - **Shield = DDoS protection**
    - **WAF = Block bad requests**
    - **Inspector = Vulnerability scanning**
    - **GuardDuty = Threat detection**
    - **Macie = S3 data classification**
    - **CloudTrail = API history**
    - **CloudWatch = Monitoring**

---

# 💰 **AWS Cost & Pricing Tools**

| Service / Tool | Purpose | Key Features | Confusing Point | When to Use |
| --- | --- | --- | --- | --- |
| **AWS Pricing Calculator** | Estimate cost before deploying | Web-based calculator, service-wise estimates, region-based pricing | Many think it shows the "actual bill," but it’s only an **estimate** | Before launching workloads to estimate monthly/yearly cost |
| **AWS Cost Explorer** | Visualize and analyze costs & usage | Graphs, trends, filters by service/region | Confusion with Billing Dashboard; this is **analysis**, not actual billing | To analyze spending patterns and optimize |
| **AWS Budgets** | Set custom cost & usage alerts | Alerts on exceeding budgets, forecast-based alerts | People confuse with Cost Explorer; Budgets = **alerts**, not analysis | To control and get notified if usage/costs exceed threshold |
| **AWS Cost Anomaly Detection** | ML-powered anomaly detection in spend | Detects unusual spikes in cost | Confused with Budgets; but this is **automatic anomaly detection**, not manual thresholds | For proactive cost anomaly alerts |
| **Billing Dashboard** | View real bills | Shows actual charges, linked accounts summary | Many think Cost Explorer = Billing Dashboard, but this shows **real bills only** | To pay/view exact charges |
| **Consolidated Billing (in AWS Organizations)** | Combine bills for multiple accounts | One bill for many accounts, volume discounts | People confuse with IAM roles; this is only for **cost aggregation** | For managing costs in multi-account setups |
| **Savings Plans** | Flexible pricing model for compute | Lower price for 1–3 year commitment; applies to EC2, Fargate, Lambda | Confused with Reserved Instances; Savings Plans = **flexible commitment** | If workloads vary but need long-term savings |
| **Reserved Instances (RI)** | Discounted pricing for EC2 | 1 or 3 year commitment; region-specific | Many confuse RI with Savings Plans; RI = **less flexible, EC2 only** | If workloads are predictable and fixed |
| **Spot Instances** | Discounted EC2 using spare capacity | Up to 90% cheaper, but can be terminated anytime | Confused with On-Demand; Spot = **unreliable, best-effort** | For fault-tolerant & flexible workloads |
| **On-Demand Instances** | Pay-as-you-go EC2 | No commitment, hourly/second billing | Confusion with RI; On-Demand = **most expensive but flexible** | For short, unpredictable workloads |
| **Free Tier** | Free usage limits for new accounts | 12-month, Always Free, and Trial categories | Many confuse "Always Free" vs "12-Month Free Tier" | For testing and learning with limited usage |

---

⚡Tip:

- Think of **Pricing Calculator** as *planning*, **Cost Explorer** as *analysis*, **Budgets** as *alerts*, and **Billing Dashboard** as *the real bill*.
- For compute pricing: **On-Demand > RI > Savings Plans > Spot** in flexibility & pricing order.

---

# 📌 AWS VPC Services Comparison (Cloud Practitioner)

| Service | Scope | Purpose | Stateful / Stateless | Inbound / Outbound | Default Behavior | Exam Keywords |
| --- | --- | --- | --- | --- | --- | --- |
| **VPC** | Region-wide | Isolated network with CIDR block | N/A | N/A | Default VPC created in each region | *Isolated network, CIDR block* |
| **Subnet** | Within a VPC | Divide VPC into public/private segments | N/A | N/A | Public + private subnets possible | *Public vs Private* |
| **Route Table** | Subnet level | Defines routing of traffic | N/A | Controls traffic destinations | One main route table per VPC | *Routing rules* |
| **Internet Gateway (IGW)** | VPC level | Provides internet access to VPC | N/A | Enables inbound & outbound internet | Must be created & attached | *Internet Access* |
| **NAT Gateway** | Subnet level | Private subnet → Internet (outbound only) | N/A | Only outbound | Must be created | *Private → Internet only* |
| **Security Group (SG)** | Instance level | Virtual firewall for EC2 | **Stateful** | Inbound + Outbound rules | Default SG allows all outbound, denies inbound | *Firewall at Instance* |
| **Network ACL (NACL)** | Subnet level | Firewall at subnet boundary | **Stateless** | Inbound + Outbound rules | Default NACL allows all traffic | *Firewall at Subnet* |
| **VPC Peering** | VPC-to-VPC | Connects two VPCs privately | N/A | Both ways | Must be set up manually | *VPC connection, no transit* |
- ⚡ **Memory Hack for Exam**
    - **VPC = Big Box**
    - **Subnets = Small Boxes inside**
    - **Route Table = Map**
    - **IGW = Door to Internet**
    - **NAT = One-way Door (private → internet)**
    - **SG = Security Guard at House (instance)**
    - **NACL = Security Guard at Colony Gate (subnet)**
    - **Peering = Bridge between colonies (VPCs)**

---

# 🔗 AWS Cloud Integration Services – Comparison Table

| **Service** | **Purpose** | **Best For** | **Key Features** | **Confusing Point** |
| --- | --- | --- | --- | --- |
| **Amazon API Gateway** | Create, publish, manage APIs | Serverless & REST/HTTP APIs | Scales automatically, security with IAM/WAF, integrates with Lambda | When to use API Gateway vs. ALB for APIs |
| **AWS AppSync** | Managed GraphQL API service | Real-time apps, mobile, IoT | Real-time data sync, offline support, GraphQL queries | Difference between AppSync (GraphQL) and API Gateway (REST) |
| **Amazon SQS (Simple Queue Service)** | Message queuing | Decoupling microservices | Standard + FIFO queues, scales automatically | Difference between SQS, SNS, and Kinesis |
| **Amazon SNS (Simple Notification Service)** | Pub/Sub messaging | Broadcasting notifications | Push to email, SMS, Lambda, SQS, apps | Difference between SNS (fan-out) vs. SQS (queueing) |
| **Amazon EventBridge (CloudWatch Events)** | Event bus for routing events | Event-driven apps | Integrates with AWS & SaaS, schema registry | Difference between EventBridge and SNS |
| **AWS Step Functions** | Workflow orchestration | Coordinating Lambda, ECS, Glue jobs | Visual workflows, retries, parallel execution | Difference between Step Functions vs. SQS + Lambda chaining |
| **AWS AppFlow** | SaaS data integration | Salesforce, Slack, Zendesk → AWS | No-code connectors, bi-directional data flow | Often confused with Data Pipeline or Glue |
| **AWS Glue** | ETL (Extract-Transform-Load) | Data lakes, analytics | Serverless ETL, integrates with Athena, Redshift | Difference between Glue and AppFlow (Glue = heavy ETL, AppFlow = SaaS sync) |
| **AWS DataSync** | Data transfer service | On-prem ↔ AWS storage | Fast transfer, incremental sync, secure | Confused with Snowball (offline transfer) |
| **AWS Direct Connect** | Dedicated network link | High bandwidth, low latency | Private connection to AWS, hybrid cloud | Difference between VPN and Direct Connect |
| **AWS VPN (Site-to-Site, Client VPN)** | Secure tunnel over internet | Hybrid cloud, user access | Site-to-Site or remote client VPN | Confusion between VPN vs. Direct Connect (VPN over internet, DX is private) |

---

- ✅ **Key Takeaways to Avoid Confusion**
    - **API Gateway vs. AppSync** → REST APIs vs. GraphQL APIs.
    - **SQS vs. SNS vs. EventBridge** → SQS = queueing, SNS = fan-out notifications, EventBridge = event routing.
    - **Step Functions vs. SQS** → Step Functions = workflows, SQS = simple messaging.
    - **AppFlow vs. Glue vs. DataSync** → AppFlow = SaaS integrations, Glue = ETL for analytics, DataSync = on-prem to cloud transfer.
    - **VPN vs. Direct Connect** → VPN = encrypted internet, Direct Connect = private dedicated line.
