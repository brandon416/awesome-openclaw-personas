# API Tester

Expert API testing specialist who ensures reliable, performant, and secure API integrations through comprehensive validation covering functional correctness, OWASP API Security Top 10, performance SLA compliance, and third-party integration resilience. Builds automated test suites with Playwright, REST Assured, and k6, integrated into CI/CD pipelines with quality gates.

## Core Capabilities

- Builds automated test suites covering functional validation (CRUD operations, input validation, error handling), security testing (auth bypass, SQL injection, rate limiting), and performance testing (response time SLAs, concurrent load)
- Tests against OWASP API Security Top 10 including authentication/authorization mechanisms, input sanitization, rate limiting, and data encryption
- Validates API performance against SLA requirements with 95th percentile response times under 200ms and error rates below 0.1% under normal load
- Tests third-party API integrations with fallback handling, error recovery, and contract compliance across service versions
- Implements contract testing with consumer-driven development, API mocking for isolated environments, and intelligent test selection based on code changes
- Produces comprehensive test reports with functional coverage, security assessment, performance metrics, and go/no-go release recommendations

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | API tester identity, security-conscious personality, experience with API failure patterns and performance bottlenecks |
| `AGENTS.md` | Security-first testing rules, performance excellence standards, integration and documentation testing requirements, four-step workflow, and success metrics |
| `SKILL.md` | Complete Playwright/JavaScript test suite example covering functional, security, and performance scenarios, deliverable report template, and advanced capabilities for penetration testing, OAuth/JWT testing, and contract testing |

## Quick Start

```bash
cp -r testing-api-tester/ ~/.openclaw/workspace/
```

## Use Cases

- Building a comprehensive API test suite for a new microservice covering authentication bypass, SQL injection prevention, and rate limiting enforcement
- Validating that all API endpoints meet a 200ms p95 response time SLA under 10x normal traffic with k6 load testing
- Testing third-party API integrations for proper fallback behavior when external services return errors, rate limit, or go down
- Integrating API security and performance tests into a CI/CD pipeline with automated quality gates that block deployment on failure
- Conducting contract testing to ensure backward compatibility when releasing a new API version
