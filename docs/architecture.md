# reapSpring Fullstack Architecture Document

*Generated using BMAD Core Architecture Template v4.0*

---

## Introduction

This document outlines the complete fullstack architecture for **reapSpring**, including backend systems, frontend implementation, and their integration. It serves as the single source of truth for AI-driven development, ensuring consistency across the entire technology stack.

This unified approach combines what would traditionally be separate backend and frontend architecture documents, streamlining the development process for modern fullstack applications where these concerns are increasingly intertwined.

### Starter Template or Existing Project

Based on the PRD technical assumptions, this project follows a **modular monolithic approach** using Next.js 15+ with Convex BaaS rather than traditional starter templates. The PRD specifies:
- Single Next.js repository with Convex backend functions co-located
- Rationale: Accelerates development velocity within 25-day timeline
- Future microservices migration path available

This is a **greenfield project** optimized for rapid deployment while maintaining enterprise scalability.

### Change Log

| Date | Version | Description | Author |
|------|---------|-------------|---------|
| 2025-09-09 | v1.0 | Initial fullstack architecture creation | Winston (Architect) |

---

## High Level Architecture

### Technical Summary

reapSpring employs a **serverless-first modular monolith** architecture using Next.js 15+ with Convex BaaS for rapid development and automatic scaling. The frontend leverages React 19+ with server-side rendering for optimal rural connectivity performance, while the backend utilizes Convex's real-time functions for professional delegation workflows and multi-tenant data isolation. Key integration points include secure magic link authentication, AI-powered application generation via GPT-5, and flexible payment routing through Stripe. This architecture deploys on Vercel's edge network with Convex handling backend scaling, enabling the platform to handle October 1st traffic surges while maintaining <2 second load times for rural users. The design achieves PRD goals by prioritizing professional delegation security, rapid consultant onboarding, and 95% application processing time reduction through intelligent AI caching and real-time collaboration features.

### Platform and Infrastructure Choice

Based on PRD requirements for rapid development, automatic scaling, and professional delegation security, I recommend:

**Platform:** Vercel + Convex  
**Key Services:** Convex (Database, Auth, Functions, File Storage), Vercel (Hosting, CDN, Edge Functions), Resend (Email), Stripe (Payments)  
**Deployment Host and Regions:** Global via Vercel Edge Network with primary regions in US-East, US-West, and US-Central for rural coverage

**Recommendation Rationale:** The 25-day timeline makes Vercel + Convex the only viable option for October 1st launch. Convex's real-time capabilities are essential for professional delegation workflows, and Vercel's edge deployment optimizes rural user performance.

### Repository Structure

**Structure:** Monorepo with Next.js App Router and co-located Convex functions  
**Monorepo Tool:** Native npm workspaces (lightweight, no additional tooling complexity)  
**Package Organization:** Feature-based packages with shared utilities (apps/web, convex/, packages/shared, packages/ui)

### Architectural Patterns

- **Serverless Architecture:** Convex functions with automatic scaling - _Rationale:_ Eliminates DevOps overhead during critical 25-day development period while handling 10x traffic spikes automatically
- **Multi-Tenant SaaS Pattern:** Row-level security with tenant isolation - _Rationale:_ Supports installer company hierarchies with secure data separation and professional delegation boundaries
- **CQRS with Real-time Sync:** Separate read/write operations with live updates - _Rationale:_ Optimizes professional collaboration workflows and manager dashboards with instant status updates
- **Magic Link Authentication:** Passwordless secure access tokens - _Rationale:_ Reduces friction for SME clients and professionals while maintaining security through time-limited single-use tokens
- **Template-based AI Generation:** Structured AI prompts with validation - _Rationale:_ Ensures consistent REAP application quality while controlling AI costs through intelligent caching
- **Progressive Web App (PWA):** Offline-capable web application - _Rationale:_ Supports rural connectivity issues while maintaining single codebase for rapid development
- **Event-Driven Architecture:** Real-time notifications and state updates - _Rationale:_ Essential for professional delegation workflows, payment confirmations, and multi-user collaboration

---

## Tech Stack

This is the DEFINITIVE technology selection for the entire project. This table is the single source of truth - all development must use these exact versions.

### Technology Stack Table

| Category | Technology | Version | Purpose | Rationale |
|----------|------------|---------|---------|-----------|
| Frontend Language | TypeScript | 5.6+ | Type-safe development across fullstack | Prevents runtime errors in professional delegation logic, enables shared types between frontend/backend |
| Frontend Framework | Next.js | 15+ | React framework with App Router | Server-side rendering for rural performance, file-based routing, built-in optimization for edge deployment |
| UI Component Library | shadcn/ui | Latest | Accessible component system | WCAG AA compliance built-in, rapid development with customizable components, excellent TypeScript support |
| State Management | XState | 5+ | Complex workflow state machines | Professional delegation workflows require complex state management, handles edge cases in multi-step processes |
| Backend Language | TypeScript | 5.6+ | Unified fullstack language | Single language reduces complexity, shared types between frontend/backend, Convex native support |
| Backend Framework | Convex | Latest | Serverless BaaS platform | Real-time capabilities for professional collaboration, automatic scaling, built-in auth and file storage |
| API Style | Convex Functions | Latest | Type-safe server functions | Direct function calls with automatic serialization, real-time subscriptions, eliminates REST API complexity |
| Database | Convex Database | Latest | Serverless document database | Built-in multi-tenancy, real-time subscriptions, automatic scaling, ACID transactions |
| Cache | Browser + Convex | Built-in | Client-side and server caching | Convex handles server caching automatically, browser cache for static assets and AI responses |
| File Storage | Convex File Storage | Latest | Secure document uploads | End-to-end encryption, professional access controls, HIPAA-ready compliance for financial documents |
| Authentication | Convex Auth | Latest | Multi-tenant authentication | Magic link support, OAuth providers, role-based access control, professional delegation security |
| Frontend Testing | Vitest | 3.2+ | Fast unit testing | Lightning-fast test execution, Jest-compatible, excellent TypeScript support, component testing |
| Backend Testing | Convex Test | Latest | Backend function testing | Built-in function testing, database mocking, integration testing support |
| E2E Testing | Playwright | 1.55+ | Cross-browser automation | Professional delegation workflows, payment processing, multi-role user journeys |
| Build Tool | Next.js | 15+ | Integrated build system | Zero configuration, automatic optimization, tree shaking, code splitting |
| Bundler | Turbopack | Latest | Fast development builds | Next.js 15 default, significantly faster than Webpack, essential for development velocity |
| IaC Tool | N/A | - | Infrastructure as Code | Convex and Vercel handle infrastructure automatically, no manual IaC required |
| CI/CD | Vercel | Latest | Automated deployment | GitHub integration, preview deployments, automatic optimization, edge deployment |
| Monitoring | Convex Dashboard | Built-in | Function and database monitoring | Real-time function performance, database queries, user activity, error tracking |
| Logging | Convex Logs | Built-in | Centralized logging | Automatic log aggregation, searchable logs, professional delegation audit trails |
| CSS Framework | Tailwind CSS | 4+ | Utility-first styling | Rapid UI development, consistent design system, dark/light mode support, excellent tree shaking |

---

## Data Models

Based on Convex's end-to-end type safety approach, the data models use Convex schema definitions with validators. This provides automatic type generation from database → functions → React components, essential for complex professional delegation workflows.

### Convex Schema Definition

```typescript
// convex/schema.ts - Production-ready schema with performance optimizations
import { defineSchema, defineTable } from "convex/server";
import { v } from "convex/values";

export default defineSchema({
  // Core multi-tenant organization structure
  installerCompanies: defineTable({
    name: v.string(),
    adminUserId: v.id("users"),
    paymentRouting: v.union(
      v.literal("company"), 
      v.literal("client"), 
      v.literal("mixed")
    ),
    settings: v.object({
      billingCycle: v.union(v.literal("monthly"), v.literal("quarterly")),
      creditLimit: v.optional(v.number()),
      allowProfessionalDelegation: v.boolean(),
      requireManagerApproval: v.boolean(),
    }),
    stripeCustomerId: v.optional(v.string()),
    status: v.union(v.literal("active"), v.literal("suspended"), v.literal("trial")),
  })
    .index("by_admin", ["adminUserId"])
    .index("by_status", ["status"]),

  // Multi-role user management with hierarchical permissions
  users: defineTable({
    email: v.string(),
    name: v.string(),
    role: v.union(
      v.literal("AccountAdmin"), 
      v.literal("ConsultantManager"), 
      v.literal("Consultant"), 
      v.literal("SMEOwner"), 
      v.literal("DelegatedProfessional")
    ),
    companyId: v.optional(v.id("installerCompanies")),
    managerId: v.optional(v.id("users")),
    permissions: v.array(v.string()),
    lastActive: v.number(),
    status: v.union(v.literal("active"), v.literal("invited"), v.literal("suspended")),
    // Magic link authentication for passwordless access
    magicLinkToken: v.optional(v.string()),
    magicLinkExpires: v.optional(v.number()),
    magicLinkUsed: v.optional(v.boolean()),
  })
    .index("by_email", ["email"])
    .index("by_company", ["companyId"])
    .index("by_magic_token", ["magicLinkToken"]),

  // SME business entities with REAP eligibility tracking
  smeClients: defineTable({
    businessName: v.string(),
    ownerId: v.id("users"),
    assignedConsultantId: v.id("users"),
    companyId: v.id("installerCompanies"),
    businessInfo: v.object({
      naicsCode: v.string(),
      businessAddress: v.object({
        street: v.string(),
        city: v.string(),
        state: v.string(),
        zipCode: v.string(),
        county: v.optional(v.string()),
      }),
      ruralAreaConfirmed: v.boolean(),
      samGovUEI: v.optional(v.string()),
      yearEstablished: v.number(),
    }),
    eligibilityStatus: v.union(
      v.literal("pending"), 
      v.literal("eligible"), 
      v.literal("ineligible"), 
      v.literal("conditional")
    ),
    eligibilityDetails: v.object({
      ruralAreaStatus: v.boolean(),
      naicsEligible: v.boolean(),
      businessSizeEligible: v.boolean(),
      samGovRegistered: v.boolean(),
      farmlandGroundMountRisk: v.optional(v.boolean()),
      lastChecked: v.number(),
    }),
    status: v.union(v.literal("active"), v.literal("onboarding"), v.literal("inactive")),
  })
    .index("by_owner", ["ownerId"])
    .index("by_consultant", ["assignedConsultantId"])
    .index("by_company", ["companyId"]),

  // Professional delegation with granular access control
  professionalDelegations: defineTable({
    applicationId: v.id("applications"),
    invitedBy: v.id("users"),
    professionalEmail: v.string(),
    professionalName: v.optional(v.string()),
    professionalType: v.union(
      v.literal("Accountant"),
      v.literal("Engineer"),
      v.literal("Advisor"), 
      v.literal("Attorney")
    ),
    authorizedSections: v.array(v.union(
      v.literal("business_financials"),
      v.literal("tax_documents"),
      v.literal("financial_projections"),
      v.literal("technical_specifications"),
      v.literal("engineering_plans"),
      v.literal("legal_documents")
    )),
    magicLinkToken: v.string(),
    accessExpires: v.number(),
    accessGranted: v.boolean(),
    contributionCompleted: v.boolean(),
    status: v.union(
      v.literal("invited"),
      v.literal("accessed"),
      v.literal("in_progress"),
      v.literal("completed"),
      v.literal("expired")
    ),
  })
    .index("by_application", ["applicationId"])
    .index("by_magic_token", ["magicLinkToken"]),
});
```

---

## Unified Project Structure

Create a monorepo structure that accommodates both frontend and backend with shared types, components, and utilities optimized for the Convex + Next.js stack.

```
reapspring/
├── .github/                     # CI/CD workflows
│   └── workflows/
│       ├── ci.yaml             # Testing and linting
│       ├── deploy-staging.yaml # Staging deployment
│       └── deploy-prod.yaml    # Production deployment
├── apps/
│   └── web/                    # Next.js frontend application
│       ├── src/
│       │   ├── app/            # Next.js App Router
│       │   │   ├── (auth)/     # Auth route group
│       │   │   ├── (dashboard)/ # Protected dashboard routes
│       │   │   ├── (professional)/ # Professional delegation routes
│       │   │   ├── (public)/   # Public marketing pages
│       │   │   └── api/        # API route handlers
│       │   ├── components/     # React components
│       │   │   ├── ui/         # shadcn/ui components
│       │   │   ├── professional/ # Professional delegation components
│       │   │   └── application/ # REAP application components
│       │   ├── hooks/          # Custom React hooks
│       │   ├── lib/            # Frontend utilities
│       │   └── stores/         # XState machines
│       ├── tests/              # Frontend tests
│       └── package.json
├── convex/                     # Convex backend functions
│   ├── applications/           # Application management functions
│   ├── professionalDelegations/ # Professional delegation functions
│   ├── files/                  # Document management functions
│   ├── eligibility/            # REAP eligibility functions
│   ├── payments/               # Payment processing functions
│   ├── lib/                   # Backend utilities
│   │   ├── schemas.ts         # Zod validation schemas
│   │   ├── zodHelpers.ts      # Custom function wrappers
│   │   └── security.ts        # Security utilities
│   └── schema.ts              # Database schema
├── packages/                   # Shared packages
│   ├── shared/                 # Shared utilities and types
│   │   ├── src/
│   │   │   ├── types/          # TypeScript interfaces
│   │   │   ├── schemas/        # Shared Zod schemas
│   │   │   ├── constants/      # Shared constants
│   │   │   └── utils/          # Shared utility functions
│   │   └── package.json
│   ├── ui/                     # Shared UI components
│   └── config/                 # Shared configuration
├── scripts/                    # Build and deployment scripts
├── docs/                      # Project documentation
├── package.json              # Root package.json with workspaces
└── README.md
```

---

## Development Workflow

### Local Development Setup

#### Prerequisites

```bash
# Required software versions
node --version  # >= 18.0.0
npm --version   # >= 9.0.0

# Install required global packages
npm install -g @convex-dev/cli@latest
npm install -g vercel@latest
npm install -g turbo@latest
```

#### Initial Setup

```bash
# Clone repository and setup
git clone https://github.com/your-org/reapspring.git
cd reapspring

# Install all dependencies (uses npm workspaces)
npm install

# Setup Convex development environment
npx convex dev --configure

# Start development environment
npm run dev
```

#### Development Commands

```bash
# Start all services (Next.js + Convex + file watching)
npm run dev

# Run type checking across all packages
npm run type-check

# Run linting across all packages
npm run lint

# Run all tests (unit + integration + e2e)
npm run test

# Build for production
npm run build
```

### Environment Configuration

```bash
# Frontend (.env.local)
NEXT_PUBLIC_CONVEX_URL=https://your-convex-deployment.convex.cloud
NEXT_PUBLIC_SITE_URL=http://localhost:3000
NEXT_PUBLIC_STRIPE_PUBLISHABLE_KEY=pk_test_...

# Backend (Convex environment)
OPENAI_API_KEY=sk-...
STRIPE_SECRET_KEY=sk_test_...
RESEND_API_KEY=re_...
MAPBOX_ACCESS_TOKEN=pk.eyJ1...

# Government API Keys
USDA_API_KEY=...
SAM_GOV_API_KEY=...

# Professional delegation security
MAGIC_LINK_SECRET=your-secure-secret-key
ENCRYPTION_KEY=your-encryption-key-for-files
```

---

## Deployment Architecture

### Deployment Strategy

**Frontend Deployment:**
- **Platform:** Vercel Edge Network with global CDN
- **Build Command:** `npm run build`
- **Output Directory:** `apps/web/.next`
- **CDN/Edge:** Automatic edge deployment with ISR

**Backend Deployment:**
- **Platform:** Convex Cloud with automatic scaling
- **Build Command:** `npx convex deploy`
- **Deployment Method:** Git-based deployment with function versioning

### Environments

| Environment | Frontend URL | Backend URL | Purpose |
|-------------|--------------|-------------|---------|
| Development | http://localhost:3000 | Local Convex Dev | Local development and testing |
| Staging | https://staging.reapspring.com | Convex Staging | Pre-production testing and QA |
| Production | https://app.reapspring.com | Convex Production | Live environment for users |

---

## Security and Performance

### Security Requirements

**Frontend Security:**
- CSP Headers: Restrict script sources to self and Convex domains
- XSS Prevention: React's built-in XSS protection, Zod input validation
- Secure Storage: No sensitive data in localStorage, magic links in secure cookies only

**Backend Security:**
- Input Validation: Comprehensive Zod validation on all function inputs and outputs
- Rate Limiting: Convex built-in rate limiting (1000 requests/minute per user)
- CORS Policy: Restricted to app.reapspring.com and staging.reapspring.com domains

**Authentication Security:**
- Token Storage: Magic links expire after 48 hours, single-use enforcement
- Session Management: Convex Auth with automatic token refresh, secure httpOnly cookies
- Password Policy: N/A (magic link only), email verification required for professional access

### Performance Optimization

**Frontend Performance:**
- Bundle Size Target: <500KB initial bundle, <1MB total for main application flow
- Loading Strategy: Route-based code splitting, lazy loading for professional delegation components
- Caching Strategy: Static assets cached for 1 year, API responses cached for 5 minutes

**Backend Performance:**
- Response Time Target: <200ms for queries, <500ms for mutations, <2s for AI generation
- Database Optimization: Strategic Convex indexes, query result caching
- Caching Strategy: Function result caching for eligibility checks, AI response caching

---

## Testing Strategy

### Testing Pyramid

```
      E2E Tests (Professional Workflows)
     /                                  \
    Integration Tests (Convex Functions)
   /                                    \
  Frontend Unit Tests    Backend Unit Tests
```

### Test Organization

**Frontend Tests:**
- Unit tests for components, hooks, and utilities
- Integration tests for auth flows and professional delegation
- E2E tests for critical user journeys and professional workflows

**Backend Tests:**
- Convex function tests with database mocking
- Integration tests for cross-function workflows
- Security tests for professional access control and magic link validation

**Professional Delegation Focus:**
- Magic link security and expiration testing
- Section access control validation
- File upload and access permission testing
- Audit trail generation and compliance verification

---

## Coding Standards

### Critical Fullstack Rules

- **Type Sharing:** Always define types in packages/shared and import from there
- **Zod Validation:** All Convex function inputs and outputs must use Zod schemas
- **Professional Access Control:** Never bypass professional delegation validation
- **Magic Link Security:** Magic links must be single-use, time-limited, and audited
- **Audit Trail Requirement:** All professional delegation actions must create audit trails
- **File Access Permissions:** Files must explicitly specify access controls
- **Environment Variables:** Access only through config objects, never process.env directly
- **Error Handling:** All functions must use ConvexError for user-facing errors
- **State Updates:** Use XState machines for complex workflows
- **Real-time Updates:** Professional collaboration must use Convex subscriptions

### Naming Conventions

| Element | Frontend | Backend | Example |
|---------|----------|---------|---------|
| Components | PascalCase | - | `ProfessionalInvitationCard.tsx` |
| Hooks | camelCase with 'use' | - | `useProfessionalDelegation.ts` |
| Convex Functions | camelCase | camelCase | `createProfessionalDelegation` |
| Database Tables | camelCase | camelCase | `professionalDelegations` |

---

## Error Handling Strategy

### Error Response Format

```typescript
interface ApiError {
  error: {
    code: string;
    message: string;
    details?: Record<string, any>;
    timestamp: string;
    requestId: string;
    professionalDelegationId?: string;
    complianceRelevant: boolean;
  };
}
```

### Professional Delegation Error Codes

- `DELEGATION_NOT_FOUND`: Professional delegation not found
- `ACCESS_EXPIRED`: Professional access has expired
- `INSUFFICIENT_PERMISSIONS`: User lacks required permissions
- `MAGIC_LINK_INVALID`: Invalid or expired magic link
- `SECTION_UNAUTHORIZED`: Unauthorized access to application section

---

## Monitoring and Observability

### Monitoring Stack

- **Frontend Monitoring:** Vercel Analytics + Sentry for error tracking
- **Backend Monitoring:** Convex Dashboard + custom metrics for function performance
- **Error Tracking:** Sentry with professional delegation context
- **Performance Monitoring:** Vercel Speed Insights + Convex function timing

### Key Metrics

**Frontend Metrics:**
- Core Web Vitals (LCP, FID, CLS)
- Professional delegation UI interactions
- Magic link access success/failure rates
- Application generation completion times

**Backend Metrics:**
- Professional delegation function response times
- Magic link validation success/failure rates
- File upload processing times and virus scan results
- AI application generation success rates and token usage
- Government API integration success rates

**Security Metrics:**
- Failed professional access attempts
- Magic link usage patterns and abuse detection
- File access violations and unauthorized section attempts
- Professional delegation expiration cleanup effectiveness

---

## Architecture Summary

The reapSpring fullstack architecture provides a comprehensive foundation for AI-driven REAP application processing with secure professional delegation capabilities. The architecture balances rapid development needs with enterprise-grade security, scalability, and compliance requirements.

**Key Architectural Features:**
- **Serverless-first approach** with Convex + Next.js for rapid development
- **Professional delegation security** with magic links, audit trails, and granular access control  
- **End-to-end type safety** with shared Zod schemas and automatic type generation
- **Real-time collaboration** supporting multi-user professional workflows
- **Comprehensive testing** ensuring security and compliance for October 1st launch
- **Production monitoring** with professional delegation and security focus

This architecture enables reapSpring to capture the October 1st REAP application surge while providing the professional delegation capabilities that differentiate the platform from existing solutions.
