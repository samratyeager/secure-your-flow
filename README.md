# SecYourFlow

**Unified Security Posture Management Platform**

Consolidate security signals from scanners, CVE feeds, and compliance frameworks into actionable intelligence.

---

## What is SecYourFlow?

SecYourFlow is a unified security posture management platform designed to streamline security operations through intelligent automation and AI-powered assistance. It consolidates security signals from scanners, CVE feeds, and compliance frameworks into actionable intelligence while reducing manual effort through automated workflows and data entry.

With an integrated RAG-powered AI chatbot, SecYourFlow enables security teams to interact with platform information, retrieve relevant insights, and get contextual answers. By combining centralized security visibility, automated processes, and intelligent assistance, it helps teams make faster, more informed, and data-driven security decisions.

```text
→ What assets are exposed and most critical?
→ Which vulnerabilities are actively exploited and require immediate attention?
→ How do current risks affect compliance frameworks (ISO 27001, NIST, PCI DSS)?
→ What actions will reduce business risk most effectively?
```

---

## Key Features

### Asset Inventory

Centralized inventory management for comprehensive asset visibility across your infrastructure.

- Servers, applications, domains, and cloud resources
- Asset criticality scoring and exposure classification
- Environment tagging (production, staging, internal)

### Vulnerability Management

Unified vulnerability tracking across multiple security scanners.

- Import from Nessus, OpenVAS, Nmap, Trivy, and more
- Normalized vulnerability model for consistent analysis
- De-duplication and remediation lifecycle tracking

### Threat Intelligence

Real-time CVE enrichment with actionable threat context.

- EPSS exploit probability scoring
- CISA KEV integration for known exploited vulnerabilities
- Source references and publication timelines

### Risk Scoring

Intelligent composite risk assessment based on multiple factors.

- CVSS severity analysis
- Asset criticality weighting
- Exposure context evaluation
- Threat signal integration (EPSS, KEV, exploitation status)

### Compliance Mapping

Framework alignment and automated gap analysis.

- ISO 27001, NIST, PCI DSS support
- Automated control coverage mapping
- Audit-ready compliance reporting

### Executive Dashboard

Business-focused security insights for leadership.

- Real-time exposure and exploitation visibility
- Risk trend analysis and forecasting
- Prioritized remediation recommendations

---

## Technology Stack

**Frontend**

- Next.js 15 with React 19
- TypeScript for type safety
- TailwindCSS for styling
- Recharts for data visualization
- Fully responsive design

**Backend**

- Next.js API Routes
- RESTful API architecture
- NextAuth.js with JWT authentication
- Role-Based Access Control (RBAC)
- Comprehensive audit logging

**Data Layer**

- PostgreSQL 16 as primary database
- Prisma ORM for type-safe queries
- Redis for caching and performance
- Real-time data synchronization

**Security Data Sources**

- NVD CVE Feeds
- EPSS (Exploit Prediction Scoring System)
- CISA KEV (Known Exploited Vulnerabilities)
- MITRE CVE Program API
- Scanner integrations (JSON import + manual findings)


## Security Architecture

SecYourFlow implements enterprise-grade security controls to protect your data and operations.

### Authentication & Authorization

- NextAuth.js with JWT strategy
- Role-Based Access Control (RBAC) with granular permissions
- Two-Factor Authentication (2FA/TOTP) with encrypted secrets at rest

### Access Roles

| Role           | Description                                      |
| -------------- | ------------------------------------------------ |
| `MAIN_OFFICER` | Executive oversight with full system access      |
| `IT_OFFICER`   | Asset and infrastructure management              |
| `PENTESTER`    | Vulnerability assessment and penetration testing |
| `ANALYST`      | Risk analysis and security reporting             |

### Security Controls

- Comprehensive audit logging for all critical actions
- Secure secret handling (no credentials stored in repository)
- Session management with automatic expiration
- Input validation and sanitization across all endpoints
- SQL injection prevention via Prisma ORM


## Project Structure

```text
secyourflow/
├── prisma/              # Database schema and migrations
├── public/              # Static assets
├── src/
│   ├── app/            # Next.js app directory
│   ├── components/     # React components
│   ├── lib/            # Utility functions and helpers
│   └── types/          # TypeScript type definitions
├── .env.example        # Environment variable template
├── docker-compose.yml  # Docker configuration
└── package.json        # Project dependencies
```

---

## Contributing

This is a private and proprietary project. Contributions are limited to authorized team members only.


*Private and proprietary. All rights reserved.*

\</div>
