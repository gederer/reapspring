# Project Brief: reapSpring

*Generated using BMAD Core Project Brief Template v2.0*

---

## Introduction

This project brief documents **reapSpring**, an AI-powered platform that automates REAP (Rural Energy for America Program) grant applications for the renewable energy industry. The brief serves as the foundational input for product development and captures the critical market opportunity created by the solar industry's transition from residential to commercial markets.

**Brief Status:** In development using interactive collaborative approach
**Last Updated:** September 8, 2025
**Next Milestone:** October 1, 2025 launch deadline (25 days)

---

## Executive Summary

**reapSpring** is a web and mobile SaaS application that automates REAP (Rural Energy for America Program) grant applications using AI technology. The platform serves the $35+ million REAP grant application preparation market by reducing application time from 1-2 weeks to minutes/hours while cutting costs from $1,500-3,500 per application to a flat $50 fee.

**Market Opportunity & Timing:**
The platform addresses a critical market inflection point: the expiration of the 30% federal residential solar tax credit will force approximately 10,000 US solar installers to pivot toward commercial markets where federal incentives remain robust. REAP grants provide 25% cost-share funding (up to $1M per project) for renewable energy systems serving small-to-medium enterprises in rural areas (population <50,000). With over 6 million qualifying SMEs nationwide and current consultant capacity severely limited, demand for application services is poised for explosive growth that existing providers cannot meet.

**Customer Segments (Who Pays):**
- **Primary Customer:** **Installer Companies** - Solar installation companies purchasing platform access for their consultant teams (~10,000 companies)
  - May also pay for applications on behalf of SME owners they invite (configurable by Account Admin/Consultant Manager)
- **Secondary Customer:** **Rural SME Owners** - Small-to-medium enterprises in rural areas applying for REAP funding (~6 million potential, ~500K+ addressable)
  - **Self-service SMEs:** Pay directly when accessing platform independently 
  - **Installer-referred SMEs:** May pay directly or have Installer Company pay on their behalf (based on company configuration)

**User Roles (Who Uses the Platform):**
- **Account Admins:** Installer company administrators managing company details, billing, and all users within their company (~10,000+ admins)
- **Renewable Energy Consultants:** Individual consultants employed by installer companies (~15,000-20,000 professionals)
- **Consultant Managers:** Management personnel overseeing consultant teams within installer companies
- **SME Owners:** Rural business owners with persistent accounts who upload documents and review applications
- **Delegated Professionals:** Accountants, business advisors, and other professionals invited by SME owners to provide specific data on their behalf

**Solution Architecture:**
reapSpring captures the complete REAP application lifecycle through guided workflows:
- **Eligibility verification:** NAICS code validation, rural area confirmation, SAM.gov registration status
- **Document management:** 3 years historical financials + 2 years projections, energy usage data, system specifications
- **AI-powered optimization:** Automatic scoring optimization (50-150% energy offset sweet spot, agricultural bonus points, farmland ground-mount rejection prevention)
- **Submission preparation:** Government-ready application packages with supporting documentation

**Value Proposition Quantified:**
- **Cost reduction:** 97% cost savings ($3,500 → $50 average)
- **Time compression:** 95% time reduction (2 weeks → 2 hours average)
- **Quality improvement:** AI-driven optimization for higher approval rates
- **Market access:** Democratizes REAP applications for underserved rural SMEs
- **Scalability:** Supports explosive demand growth beyond human consultant capacity

**Revenue Model:** 
Flat $50 per application with flexible payment routing:
- **Direct SME Payment:** Individual SME owners pay $50 per application
- **Installer Company Payment:** Companies may pay $50 per application on behalf of referred SME clients (configurable setting)
- **Enterprise Pricing:** Potential tiered pricing for high-volume installer companies managing multiple applications
- **Target Volume:** 50,000-100,000 applications annually within 3 years

---

## Problem Statement

**MISSION-CRITICAL TIMELINE:** reapSpring must launch by **October 1, 2025** - exactly **25 days from now** - to capture the REAP FY 2026 market opening.

### Current State and Pain Points

**1. IMMINENT MARKET EXPLOSION - 25 DAYS**
REAP FY 2026 applications open **October 1, 2025** with the largest funding opportunity in program history. The program is currently paused, creating maximum pent-up demand that will flood the market in exactly 25 days. **Missing this launch window means missing the primary market opportunity entirely.**

**2. Enhanced Funding Creates Surge Demand**  
The Inflation Reduction Act **doubled** available funding - IRA grants now cover up to **50%** of project costs. This will create unprecedented application volume starting October 1st, with three critical deadlines creating massive consultant bottlenecks.

**3. Program Sustainability Concerns**
REAP funding faces periodic appropriation challenges, and current beneficiaries remain largely unengaged in the political process. **A brief, educational reminder about civic engagement could help ensure program continuity** without creating compliance issues.

**4. Critical Application Rejection Risk**
**Ground-mounted solar systems on farmland face automatic REAP application rejection**, creating a major compliance trap that consultants must avoid. Current manual processes lack systematic checks for this critical requirement, leading to wasted time and disappointed SME clients.

**5. Industry Crisis: No Time for Training**
10,000 solar installer companies with 15,000-50,000+ consultants face an impossible situation: they must pivot to commercial REAP expertise in **25 days** or lose market access entirely. Traditional training/mentorship cannot scale to this timeline.

**6. Prohibitive Cost Barrier Will Intensify**
Current consultants charge $1,500-3,500 per application. With surge demand hitting unprepared consultants on October 1st, prices will spike dramatically while availability plummets. Most SMEs will be priced out entirely.

**7. Complex Domain Knowledge Gap**
REAP applications require specialized knowledge of federal regulations, NAICS classifications, rural area definitions, SAM.gov/UEI processes, dual funding streams (IRA vs. Farm Bill), financial projections, and energy optimization. **Zero consultants can master this in 25 days.**

### Impact Quantification

- **Timeline crisis:** 25 days to prepare for program reopening
- **Market access crisis:** Entire consultant workforce unprepared for October 1st surge
- **Revenue crisis:** Solar companies face potential revenue collapse without commercial pivot tools
- **Opportunity cost:** Missing October 1st means 12+ month wait for next major market catalyst

### Why Existing Solutions Are Impossible

**Time has eliminated all alternatives.** Training consultants, building manual processes, hiring REAP experts - none can scale to 15,000-50,000 professionals in 25 days. The market needs an immediate, scalable solution that democratizes REAP expertise instantly.

### Urgency and Importance

**This is a 25-day sprint to market capture.** The combination of program reopening + enhanced funding + consultant unpreparedness creates a winner-take-most scenario. The first scalable solution to market captures the entire industry transition. **There is no second chance - the market explodes on October 1st with or without us.**

---

## Proposed Solution

**reapSpring transforms REAP grant application preparation from a specialized consulting bottleneck into an accessible, automated, AI-powered platform that can serve the entire market within our 25-day launch window.**

### Core Concept and Approach

**1. AI-Powered Application Generation Engine**
- **Intelligent document processing** that extracts and validates required information from uploaded financial documents, energy bills, and system specifications
- **Automated eligibility verification** using real-time NAICS code lookup, rural area confirmation via USDA databases, and SAM.gov registration status checking
- **Smart application optimization** that automatically calculates optimal system sizing (50-150% energy offset), identifies agricultural bonus opportunities, and prevents farmland ground-mount rejections
- **Government-ready output generation** producing complete application packages formatted exactly to USDA specifications

**2. Hierarchical Multi-Tenant Organization Structure**
- **Installer Company Accounts:** Each of the 10,000 installer companies gets a master account with company-wide settings, branding, and oversight capabilities
- **Manager Dashboards:** Consultant managers within each installer company can:
  - Oversee all consultants employed by their company
  - Monitor consultant application volume and performance metrics
  - Assign SME clients to specific consultants
  - Track company-wide REAP application pipeline and revenue
- **Consultant Workbenches:** Individual consultants get accounts linked to their employer company, providing:
  - Personal application queues and client management
  - SME client onboarding and document collection tools
  - Application generation and submission capabilities
  - Performance tracking tied to company management oversight
- **SME Client Accounts:** All SME owners receive persistent accounts with full access to:
  - **Invitation Process:** Installer companies can invite SME clients via email + SMS containing magic link for easy onboarding
  - **Authentication Options:** Sign in using email/password or OAuth providers (Google, Microsoft, etc.)
  - **Document Management:** Upload required documentation directly (financials, energy bills, system specifications)
  - **Professional Delegation:** Invite accountants, business advisors, or other professionals to provide specific data sections on their behalf
  - **Application Review:** Review complete application drafts before submission
  - **Status Tracking:** Monitor application progress through the federal review process
  - **Account Persistence:** Maintain access to historical applications and professional relationships for future use

**3. Professional Delegation System**
- **Universal Access:** Both installer-referred AND self-service SME owners can invite professional assistance
- **Granular Permissions:** SME owners can delegate specific sections (financial data, projections, technical specifications) to different professionals
- **Professional Invitation:** Invited professionals (accountants, business advisors, engineers) receive secure access links to provide only their designated data sections
- **Audit Trail:** Complete tracking of who provided which information and when, maintaining accountability for all application components
- **Professional Persistence:** Professionals can maintain relationships with multiple SME clients for ongoing REAP application assistance
- **Data Isolation:** Professionals only see the specific sections they're authorized to complete, protecting overall SME business confidentiality

**4. Dual Payment Processing Infrastructure**
- **Installer Company Payment Systems:**
  - Monthly/annual subscription billing for company accounts
  - Per-application fees ($50 per application) with bulk pricing tiers
  - Automated invoicing and payment collection
  - Company credit limits and payment terms for high-volume users
  - Manager-level payment oversight and budget controls
- **SME Owner Direct Payment:**
  - Secure credit card/ACH processing for individual SME applications
  - $50 flat fee payment at application submission
  - Payment confirmation required before final application generation
  - Receipt generation and tax documentation
- **Payment Routing Logic:**
  - System determines payment source based on application type (installer-managed vs. self-service SME)
  - Automated reconciliation between installer company accounts and individual SME payments

**5. Organizational Workflow Management**
- **Company-level billing and subscription management** for installer enterprises
- **Manager oversight tools** for tracking consultant productivity and client satisfaction
- **Consultant assignment system** allowing managers to distribute SME clients efficiently
- **Cross-consultant collaboration** for complex applications requiring specialized expertise
- **Company branding and white-label options** for installer companies serving their SME clients

**6. Domain Knowledge Democratization**
- **Embedded REAP expertise** that guides consultants through complex federal requirements without specialized training
- **Real-time validation** preventing common errors that lead to application rejections
- **Intelligent prompting** that helps consultants gather optimal information for higher approval rates
- **Educational context** explaining requirements to both consultants and their SME clients

### Key Differentiators from Existing Solutions

**Organizational Scalability:** Platform serves the entire installer company ecosystem (companies → managers → consultants → SME clients) rather than individual users, matching actual industry structure.

**Management Visibility:** Consultant managers can oversee their team's REAP pivot progress, track revenue opportunities, and ensure quality control across all applications.

**Company Integration:** Installer companies can integrate REAP services into their existing commercial solar offerings, creating new revenue streams while serving existing SME relationships.

**Efficiency Multiplier:** Single consultants can handle 10-20x more applications with AI assistance, allowing companies to serve the commercial market surge without massive hiring.

**Flexible Payment Models:** Supports both B2B (installer company) and B2C (individual SME) payment flows, maximizing market capture across all user segments.

### Why This Solution Will Succeed Where Others Haven't

**Matches Industry Structure:** Built for the actual installer company → manager → consultant → SME client relationship chain rather than generic user models.

**Enables Company Pivot:** Helps entire installer companies transition to commercial markets systematically rather than leaving individual consultants to figure it out independently.

**Manager Control:** Consultant managers get the oversight tools needed to manage their teams' transition to REAP expertise, ensuring quality and consistency.

**Preserves Relationships:** SME clients still work with their trusted installer company consultants, just with powerful AI assistance.

**Payment Flexibility:** Unlike single-payment-model competitors, reapSpring accommodates both installer company billing preferences and individual SME direct payment needs.

### High-Level Product Vision

reapSpring becomes the **standard infrastructure for installer company REAP operations**, enabling the systematic industry transition from residential to commercial solar markets. The platform supports the entire organizational hierarchy while providing **minimal civic engagement reminders** to help ensure long-term program sustainability.

**Success creates market expansion rather than market share capture** - by reducing barriers, we grow the entire REAP application market rather than just redistributing existing consultant revenue.

---

## Target Users

reapSpring serves a multi-stakeholder ecosystem centered around the installer company organizational structure, with each user segment having distinct needs, workflows, and success metrics.

### Primary User Segment: Renewable Energy Consultants

**Demographic Profile:**
- **Role:** Individual consultants employed by solar installation companies
- **Experience:** Primarily residential solar expertise, limited REAP/commercial knowledge
- **Size:** 15,000-50,000 professionals across 10,000 installer companies
- **Geographic:** Distributed nationwide, concentrated in solar-favorable markets

**Current Behaviors and Workflows:**
- Focus on residential solar installations and tax credit optimization
- Work within installer company hierarchies with manager oversight
- Manage client relationships from initial contact through installation
- Handle documentation collection, permitting, and financial qualification processes
- Currently unprepared for commercial solar/REAP transition

**Specific Needs and Pain Points:**
- **Immediate REAP expertise acquisition** without months of specialized training
- **Workflow integration** with existing client management processes
- **Manager visibility** into their REAP application performance and progress
- **Error prevention** tools to avoid federal application rejections
- **Time efficiency** to handle 10-20x more applications than manual processes

**Goals They're Trying to Achieve:**
- Successfully pivot to commercial solar markets to maintain employment
- Generate REAP application revenue to offset declining residential opportunities
- Serve existing SME client relationships with expanded service offerings
- Meet manager expectations for productivity and application quality

### Primary User Segment: Rural SME Owners

**Demographic/Firmographic Profile:**
- **Business Size:** Small-to-medium enterprises under NAICS size standards
- **Location:** Rural areas (population <50,000) across all 50 states
- **Industries:** Agriculture, manufacturing, retail, services, hospitality
- **Revenue:** Typically $500K-$10M annually, seeking $20K-$500K energy projects

**Current Behaviors and Workflows:**
- Work with trusted installer company representatives for energy projects
- Rely on professional guidance for complex federal programs and paperwork
- Focus on core business operations, not energy policy expertise
- Value relationships with local/regional service providers
- Prefer guided processes over self-service for complex applications

**Specific Needs and Pain Points:**
- **Simplified document provision** without understanding complex federal requirements
- **Trust and transparency** in application process and cost structure
- **Minimal time investment** while maintaining control over their application
- **Clear status updates** on application progress and federal review process
- **Cost predictability** ($50 vs. $1,500-3,500 consultant fees)
- **Professional delegation capability** to involve their trusted accountants/advisors

**Goals They're Trying to Achieve:**
- Access 25-50% federal funding to reduce energy system installation costs
- Work with trusted installer company representatives OR maintain independence
- Minimize administrative burden while maximizing grant award potential
- Complete applications accurately to avoid delays or rejections
- Leverage existing professional relationships (accountants, advisors) for complex data sections

### Secondary User Segment: Consultant Managers

**Demographic Profile:**
- **Role:** Management personnel overseeing consultant teams at installer companies
- **Size:** 2,000-5,000 managers across 10,000 installer companies
- **Responsibility:** Teams of 2-50+ consultants depending on company size
- **Background:** Senior consultants or business operations professionals

**Current Behaviors and Workflows:**
- Oversee consultant performance, training, and client satisfaction
- Manage company revenue targets and business development strategies
- Coordinate between consultants and company leadership
- Handle escalated client issues and quality control processes
- Currently planning commercial market pivot strategies

**Specific Needs and Pain Points:**
- **Team performance visibility** for REAP application productivity and quality
- **Training oversight** to ensure consistent consultant competency
- **Revenue tracking** for new commercial market opportunities
- **Quality control** to maintain company reputation and client satisfaction
- **Resource allocation** to optimize consultant assignments and workloads

**Goals They're Trying to Achieve:**
- Successfully manage team transition to commercial solar markets
- Maintain company revenue during residential market decline
- Ensure consistent application quality across all consultants
- Scale commercial operations to capture market opportunity

### Supporting User Segment: Account Admins

**Demographic Profile:**
- **Role:** Installer company administrators managing platform operations
- **Size:** ~10,000+ admins (1+ per installer company)
- **Responsibility:** Company-wide platform configuration, billing, and user management
- **Background:** Operations managers, IT administrators, or senior consultants

**Current Behaviors and Workflows:**
- Manage company technology platforms and software subscriptions
- Configure user permissions and access controls
- Handle billing, invoicing, and vendor relationships
- Set company policies and operational procedures
- Coordinate with external vendors and service providers

**Specific Needs and Pain Points:**
- **Simple platform configuration** for company-wide settings
- **Billing transparency** and cost control mechanisms
- **User management** tools for consultant onboarding/offboarding
- **Payment routing control** (company pays vs. client pays configuration)
- **Compliance oversight** to ensure company applications meet standards

**Goals They're Trying to Achieve:**
- Efficiently manage company transition to REAP operations
- Control costs while enabling consultant productivity
- Maintain oversight of company REAP application quality and compliance
- Streamline administrative overhead for commercial market expansion

### Supporting User Segment: Delegated Professionals

**Demographic Profile:**
- **Role:** Accountants, business advisors, engineers, and other professionals
- **Size:** Potentially 50,000+ professionals across multiple disciplines
- **Relationship:** Invited by SME owners to provide specific data sections
- **Geographic:** Distributed nationwide, often serving rural business communities

**Current Behaviors and Workflows:**
- Provide specialized services (accounting, engineering, business consulting) to rural SMEs
- Handle financial documentation, projections, and compliance requirements
- Work with multiple clients across various federal and state programs
- Maintain professional certifications and stay current on regulatory requirements
- Often serve as trusted advisors for complex business decisions

**Specific Needs and Pain Points:**
- **Secure access** to only the data sections they're authorized to complete
- **Clear scope definition** of their responsibilities within each application
- **Efficient workflow** to serve multiple SME clients without duplication
- **Professional liability protection** through proper documentation and audit trails
- **Client relationship preservation** while working within platform constraints

**Goals They're Trying to Achieve:**
- Efficiently serve multiple SME clients with REAP application assistance
- Maintain professional standards and liability protection
- Build recurring revenue through ongoing client relationships
- Expand service offerings to include federal grant application support

---

## Goals & Success Metrics

### Business Objectives

- **Launch by Market Opening:** Deploy functional MVP by October 1, 2025 (25 days) to capture REAP FY 2026 application surge
- **User Acquisition:** Onboard 500+ installer companies and 2,500+ consultants within first 90 days of launch
- **Application Volume:** Process 10,000+ REAP applications within first 12 months, targeting $500K revenue
- **Market Penetration:** Capture 20% of total REAP application market by end of Year 1 
- **Customer Retention:** Achieve 90% consultant retention rate and 85% installer company renewal rate
- **Revenue Growth:** Scale to 50,000-100,000 applications annually by Year 3, generating $2.5M-5M ARR
- **Margin Optimization:** Maintain 70%+ gross margins through intelligent cost management strategies

### Cost Optimization & Margin Management

**AI Cost Control Strategies:**
- **Intelligent Caching:** Cache frequently-used REAP content (eligibility rules, NAICS classifications, form templates) to reduce API calls by 60-80%
- **Application Component Reuse:** Template common sections (company descriptions, energy calculations, federal compliance language) across similar applications
- **Tiered AI Usage:** Use lightweight models for validation/formatting, premium models only for complex content generation
- **Batch Processing:** Group similar applications for bulk AI processing to leverage volume pricing
- **Target AI Cost:** $2-5 per application (10% of revenue) through optimization strategies

**Infrastructure Cost Management:**
- **Cloud-Native Scaling:** Auto-scaling infrastructure to handle October 1st surge without over-provisioning
- **Content Delivery Networks:** Cache static assets (forms, templates, validation rules) to reduce bandwidth costs
- **Database Optimization:** Efficient data structures to minimize storage and query costs
- **Target Hosting Cost:** $3-7 per application (15% of revenue) including compute, storage, and bandwidth

**Total Cost of Goods Sold Target:** $5-12 per application (25% of $50 revenue) leaving $38-45 gross margin

### Customer Acquisition Strategy & Metrics

**Low-Cost Installer Company Acquisition:**
- **Industry Conference Presence:** Target 3-5 major solar conferences with booth + speaking opportunities ($15K total investment)
- **Trade Publication Content Marketing:** Authored articles in Solar Power World, PV Magazine targeting commercial pivot themes
- **LinkedIn Sales Outreach:** Direct outreach to installer company owners/managers with commercial pivot messaging
- **Referral Program:** $100 credit for each successful installer company referral
- **Target Customer Acquisition Cost:** <$200 per installer company (payback in <5 applications)

**Viral SME Owner Acquisition:**
- **Installer-Driven Referrals:** Incentivize consultants to refer SME clients with application fee sharing
- **Rural Business Network Partnerships:** Partner with farm associations, rural chambers of commerce, agricultural extension offices
- **Success Story Marketing:** Case studies of successful REAP applicants shared through rural business networks
- **Local Media Coverage:** Press releases in rural newspapers highlighting successful local grants
- **Target SME Acquisition Cost:** <$10 per SME (20% of single application revenue)

### User Success Metrics

- **Consultant Productivity:** Enable individual consultants to process 20+ applications per month (vs. 2-4 manual applications)
- **Application Quality:** Achieve 85%+ REAP grant approval rate for platform-generated applications
- **Time Reduction:** Reduce application preparation time from 1-2 weeks to 2-4 hours average
- **Cost Savings:** Deliver 97% cost reduction ($3,500 → $50) compared to traditional consulting
- **User Satisfaction:** Maintain 4.5+ star rating across all user segments
- **SME Access:** Enable 50,000+ rural SMEs to apply for REAP funding who previously couldn't afford consultant fees

### Key Performance Indicators (KPIs)

**Financial KPIs:**
- **Gross Margin:** Percentage of revenue after AI and infrastructure costs (target: 70%+)
- **Customer Acquisition Cost:** Cost to acquire installer companies vs. SME owners (targets: <$200 vs. <$10)
- **Customer Lifetime Value:** Revenue per customer over 24 months (target: $2,000+ installer companies, $50+ SMEs)
- **Cost Per Application:** Total operating costs divided by applications processed (target: <$12)

**Operational KPIs:**
- **Platform Utilization:** Monthly active consultants using the platform (target: 80% of registered consultants)
- **Application Completion Rate:** Percentage of started applications that reach submission (target: 90%+)
- **Payment Conversion:** Percentage of applications that convert to paid submissions (target: 95%+)
- **Support Ticket Volume:** Customer support requests per 1,000 applications (target: <50 tickets)
- **Platform Uptime:** System availability during peak application periods (target: 99.9% uptime)
- **Federal Approval Rate:** Percentage of reapSpring applications approved by USDA (target: 85%+)

**Growth KPIs:**
- **Market Coverage:** Number of states with active installer company customers (target: 45+ states)
- **Consultant Efficiency:** Applications processed per consultant per month (target: 15+ applications)
- **Viral Coefficient:** Average number of new SME customers referred by each installer company (target: 2.0+)
- **Content Reuse Rate:** Percentage of application content generated from cached/templated sources (target: 60%+)

---

## MVP Scope

**CRITICAL CONSTRAINT:** 25 days to October 1st launch requires absolute focus on core functionality that enables immediate market capture.

### Core Features (Must Have)

- **Basic User Registration & Authentication**
  - Installer company account creation with admin user
  - Consultant account creation linked to installer company
  - SME persistent account creation with email/password and OAuth options
  - Magic link invitation system for SME onboarding via email + SMS
  - **Rationale:** Essential for multi-tenant access control, payment routing, and user workflow management

- **Professional Delegation System**
  - SME owners can invite accountants, advisors, engineers to provide specific data sections
  - Granular permissions for delegated professionals (financial data, technical specs, projections)
  - Secure access links for professionals to access only authorized sections
  - Audit trail tracking who provided which information
  - **Rationale:** Core differentiator enabling SME owners to leverage existing professional relationships

- **Simplified Application Workflow**
  - Single-page guided form for essential REAP data collection
  - Document upload for financials (3 years + 2 projections), energy bills, system specs
  - Basic eligibility validation (rural area check, NAICS lookup, basic size verification)
  - Professional delegation interface for section assignment
  - **Rationale:** Minimum viable flow to generate submittable applications with professional support

- **AI Application Generation (Basic)**
  - Template-based application assembly using uploaded data and professional inputs
  - Simple energy calculation (% offset calculation for scoring optimization)
  - Farmland ground-mount rejection prevention checks
  - PDF generation matching USDA application format requirements
  - **Rationale:** Core value proposition - AI-generated federal applications with compliance validation

- **Payment Processing**
  - Stripe integration for $50 per application payment
  - Flexible payment routing (installer company vs. individual SME vs. professional)
  - Payment confirmation before application finalization
  - Configurable payment settings managed by Account Admins
  - **Rationale:** Revenue generation essential for business viability with flexible customer models

- **Minimal Manager Dashboard**
  - View consultant application volume and status
  - Basic company-level application tracking
  - Payment routing configuration controls
  - User management for consultants within company
  - **Rationale:** Management oversight requirement for installer companies and billing control

- **Civic Engagement Reminder (Minimal)**
  - Simple post-application completion message suggesting contacting representatives
  - Link to representative lookup tool
  - **Rationale:** Compliance-safe advocacy component as specified requirement

### Out of Scope for MVP

**Advanced AI Features**
- GAN-based training system (planned for post-MVP)
- Complex optimization algorithms beyond basic energy calculations
- Multi-document intelligent parsing beyond basic data extraction
  
**Advanced User Management**
- Granular permissions and roles beyond basic user types
- Detailed user profiles and preferences
- Complex organizational hierarchies beyond company/manager/consultant structure

**Comprehensive Dashboards**
- Advanced analytics and reporting
- Detailed performance metrics and business intelligence
- Complex data visualization and trend analysis

**Integration Features**
- CRM system integrations
- Third-party document management systems
- External API connections beyond basic payment/validation/government databases

**Advanced Workflow Management**
- Multi-step application approval workflows
- Complex collaboration tools beyond professional delegation
- Advanced notification systems and automated reminders

**White-Label/Branding**
- Custom company branding and themes
- White-label platform options for installer companies
- Advanced customization features and company-specific workflows

**Advanced Professional Features**
- Professional certification tracking
- Complex professional liability documentation
- Advanced professional networking and referral systems

### MVP Success Criteria

**Functional Success:**
- Generate technically compliant REAP applications that pass initial USDA screening
- Process payments successfully for all customer types (installer companies, SMEs, professional-assisted)
- Support 100+ concurrent users during peak October 1st launch period
- Achieve <5 second application generation time for basic applications
- Successfully handle professional delegation workflows with secure access controls

**Business Success:**
- Onboard 50+ installer companies by October 31st (first month)
- Process 500+ applications by December 31st (first quarter)
- Achieve 90%+ payment conversion rate (started applications that complete payment)
- Maintain <10% support ticket rate per application
- Successfully demonstrate professional delegation value proposition

**Technical Success:**
- 99%+ uptime during October 1st launch surge
- Successful payment processing with <1% transaction failure rate
- Application PDF generation that passes USDA format validation
- Support horizontal scaling to handle 10x traffic spikes
- Secure professional delegation system with proper access controls and audit trails

---

## Post-MVP Vision

After establishing market presence with the October 1st MVP launch, reapSpring will evolve into a comprehensive rural energy ecosystem platform while maintaining focus on profitable growth.

### Phase 2 Features (Q1-Q2 2026)

**Advanced AI Application Generation**
- **GAN-based Training System:** Implement the planned generative adversarial network that trains on successful application patterns to improve generation quality and approval rates
- **Multi-Document Intelligence:** Advanced parsing of financial documents, energy audits, and technical specifications for automated data extraction
- **Optimization Engine:** Complex algorithms that maximize REAP scoring across all evaluation criteria
- **Professional AI Assistance:** AI-powered suggestions for delegated professionals to optimize their specific data sections

**Enhanced User Experience**
- **Advanced Dashboards:** Comprehensive analytics for managers tracking ROI, consultant performance, and market opportunities
- **Workflow Automation:** Automated application status tracking, deadline reminders, and document collection workflows
- **Mobile Application:** Native mobile apps for consultants to manage applications on-site with SME clients
- **Professional Networking:** Enhanced collaboration tools for delegated professionals to coordinate across applications

**Platform Scaling Features**
- **Advanced Multi-Tenancy:** White-label platform options for large installer companies with custom branding
- **API Ecosystem:** Public APIs enabling third-party integrations with CRM systems, accounting software, and project management tools
- **Advanced Payment Features:** Subscription billing, usage-based pricing tiers, and revenue sharing models for professional services
- **Professional Marketplace:** Directory of verified professionals available for delegation by SME owners

### Long-Term Vision (1-2 Years)

**Comprehensive Rural Energy Platform**
reapSpring evolves beyond REAP applications to become the central platform for all rural energy incentives and programs:
- **Multi-Program Support:** USDA Rural Development programs, state-level rural energy incentives, utility rebate programs
- **Energy Project Lifecycle:** From initial feasibility through financing, permitting, installation, and ongoing monitoring
- **Rural Energy Marketplace:** Connecting SMEs with vetted installer companies, financing options, equipment suppliers, and professional services
- **Professional Services Ecosystem:** Comprehensive network of accountants, engineers, and advisors specializing in rural energy programs

**National Market Leadership**
- **Geographic Expansion:** Comprehensive coverage across all 50 states with localized program knowledge
- **Market Penetration:** Processing 100,000+ applications annually across multiple federal and state programs
- **Industry Integration:** Standard platform used by majority of commercial solar installers for rural market operations
- **Professional Network:** Largest network of rural energy professionals and service providers

**Policy Influence Infrastructure**
- **Legislative Tracking:** Real-time monitoring of rural energy policy changes and funding opportunities
- **Advocacy Analytics:** Data-driven insights on program utilization to support policy recommendations
- **Stakeholder Network:** Organized coalition of rural energy beneficiaries for program protection and expansion
- **Professional Advocacy:** Tools and resources for professionals to engage in policy advocacy on behalf of their rural clients

### Expansion Opportunities

**Federal Grant Program Expansion**
- **USDA Rural Development Portfolio:** Value-Added Producer Grants, Rural Business Development Grants, Community Facilities Direct Loan & Grant Program
- **Department of Energy Programs:** Small Business Innovation Research (SBIR), State Energy Program grants, Weatherization Assistance Program
- **EPA Environmental Grants:** Brownfields grants, Environmental Justice grants, Pollution Prevention grants
- **SBA Small Business Grants:** Innovation Research (SBIR/STTR), Regional Innovation Clusters, Growth Accelerator Fund Competition
- **Treasury/IRS Tax Credit Programs:** Investment Tax Credit (ITC) applications, Production Tax Credit (PTC) documentation

**State and Local Grant Programs**
- **State Energy Offices:** Renewable energy incentive programs across all 50 states
- **Agricultural Departments:** Farm modernization grants, sustainable agriculture programs, rural infrastructure development
- **Economic Development Agencies:** Small business development grants, rural economic development programs, workforce development funds
- **Utility Rebate Programs:** Automated application processing for utility-sponsored energy efficiency and renewable programs

**Professional Services Expansion**
- **Specialized Grant Categories:** Non-profit sector foundation grants, research institution funding, minority and women-owned business programs
- **Cross-Program Optimization:** Intelligent recommendations for complementary grant programs SMEs may qualify for simultaneously
- **Compliance Management:** Automated tracking of diverse federal, state, and local reporting requirements across multiple active grants
- **Professional Certification:** Training and certification programs for professionals specializing in rural energy grant applications

**Market Size Implications**
- **Total Addressable Market Expansion:** From $35M REAP market to $500M+ comprehensive grant application services market
- **Customer Base Growth:** From 6M rural SMEs to 30M+ small businesses eligible for various federal and state grant programs
- **Revenue Diversification:** Reduced dependency on single program (REAP) funding cycles and political changes
- **Professional Network Scale:** From 50,000+ delegated professionals to comprehensive rural business services ecosystem

**Adjacent Market Opportunities**
- **Urban Energy Incentives:** Expand platform to serve urban commercial energy programs and incentives
- **Residential Market Return:** When new residential incentives emerge, platform ready for rapid market re-entry
- **Energy Efficiency Programs:** Beyond renewable generation to comprehensive energy efficiency incentive programs
- **International Markets:** Rural energy incentive programs in Canada, EU, and other developed markets with similar agricultural economies

**Technology Evolution**
- **Predictive Analytics:** AI models predicting application approval likelihood and optimal timing strategies across multiple grant programs
- **Advanced Data Analytics:** Comprehensive insights on program utilization patterns and success factors across federal agencies
- **Cross-Agency Intelligence:** Pattern recognition across different government agencies' evaluation criteria and preferences
- **Professional AI Assistants:** Specialized AI tools for different professional disciplines (accounting, engineering, legal) within the platform

---

## Technical Considerations

**CRITICAL TIMELINE:** All technical decisions must support functional deployment by October 1st, 2025 (25 days from now).

### Platform Requirements

**Target Platforms**
- **Web Application:** Primary platform - responsive web app accessible on desktop and mobile browsers
- **Browser Support:** Chrome, Firefox, Safari, Edge (latest 2 versions) - covers 95%+ of target user base
- **Mobile Web:** Mobile-optimized responsive design (native apps in Phase 2)
- **Performance Requirements:** <3 second page load times, <5 second application generation

### Technology Preferences

**Frontend Stack**
- **Framework:** Next.js with TypeScript for full-stack React development and team familiarity
- **UI Framework:** Tailwind CSS for fast, consistent styling and utility-first approach
- **State Management:** Zustand for lightweight client-side state (if needed - React state may suffice for MVP)
- **File Upload:** Convex direct file upload for seamless document handling (financials, energy bills, system specs)
- **PDF Generation:** React-PDF or similar for client-side application previews

**Backend & Database**
- **Backend:** Convex for backend functions, database, and real-time features
- **Database:** Convex's built-in database for all application data (users, companies, applications, professional delegations)
- **File Storage:** Convex file storage for document uploads and PDF generation
- **Authentication:** Convex Auth for user management and session handling
- **Email Services:** Resend for transactional emails and notifications (magic links, professional invitations)

**Hosting/Infrastructure**
- **Platform:** Vercel for Next.js hosting with automatic scaling and edge deployment
- **Database/Backend:** Convex hosted backend with automatic scaling
- **CDN:** Vercel's built-in CDN for global performance
- **Monitoring:** Vercel Analytics + Convex Dashboard for performance and error tracking

### Architecture Considerations

**Repository Structure**
- **Single Repository:** Next.js frontend with Convex backend functions in same repo
- **Folder Structure:** `/app` (Next.js App Router), `/convex` (backend functions), `/lib` (shared utilities)
- **Package Management:** npm or pnpm for dependency management

**Service Architecture**
- **Unified Stack:** Next.js + Convex provides full-stack solution without separate API services
- **Serverless Functions:** Convex functions handle all backend logic (auth, payments, AI integration, professional delegation)
- **Real-time Capabilities:** Convex provides reactive queries for live dashboard updates and professional collaboration

**Integration Requirements**
- **Document Upload:** Convex direct file upload API for SME financial documents and energy bills
- **Payment Processing:** Stripe integration via Convex functions for $50 application payments with flexible routing
- **AI Services:** OpenAI GPT-4 or Claude API calls from Convex functions for application generation
- **Government APIs:** USDA rural area lookup, NAICS code validation from Convex functions
- **Email Services:** Resend integration via Convex for transactional emails (magic links, professional invitations, status updates)
- **SMS Services:** Integration for magic link delivery via SMS for SME onboarding

**Security/Compliance**
- **Data Protection:** Convex handles encryption at rest and in transit automatically
- **Authentication:** Convex Auth with secure session management and user roles
- **Access Control:** Role-based permissions implemented via Convex schema and functions (professional delegation security)
- **PCI Compliance:** Stripe handles payment processing to avoid PCI requirements
- **File Security:** Convex file storage with access controls for sensitive SME documents
- **Professional Delegation Security:** Granular permissions ensuring professionals access only authorized data sections
- **Audit Trails:** Comprehensive logging of professional contributions and data access

### MVP Technical Constraints

**Development Speed Optimizations**
- **Convex Auth:** Built-in authentication system eliminates custom auth development
- **Convex File Upload:** Direct file upload to Convex eliminates need for third-party file handling
- **Template-Based AI:** Pre-built application templates with Convex functions for variable substitution
- **Unified Database:** Single Convex database for all entities reduces complexity
- **Single Deployment:** Next.js + Convex deploy together, no separate backend deployment

**Scalability Preparations**
- **Automatic Scaling:** Both Vercel and Convex handle traffic spikes automatically
- **Edge Distribution:** Vercel's global CDN ensures fast loading worldwide
- **Database Performance:** Convex's query optimization and caching built-in
- **Real-time Updates:** Convex reactive queries provide live dashboard updates for managers and professional collaboration

**Risk Mitigation**
- **Mature Stack:** Both Next.js/Vercel and Convex are production-proven platforms
- **Team Familiarity:** Using known technologies reduces development risk
- **Built-in Monitoring:** Vercel and Convex provide comprehensive observability
- **Automatic Backups:** Convex handles database backups and point-in-time recovery

### Development Advantages

**Team Productivity**
- **Familiar Technologies:** Next.js, Tailwind, Convex are well-known to development team
- **Reduced Context Switching:** Full-stack TypeScript throughout the application
- **Integrated Development:** Convex dev mode provides local development environment
- **Type Safety:** End-to-end TypeScript from frontend to backend functions

**Deployment Simplicity**
- **Single Command Deployment:** `npx convex deploy` + Vercel auto-deployment
- **No DevOps Overhead:** Managed platforms handle scaling, monitoring, backups
- **Environment Management:** Built-in staging/production environment handling

**Professional Delegation Technical Requirements**
- **Granular Access Control:** Convex schema supports fine-grained permissions for professional data section access
- **Secure Invitation System:** Magic link generation with expiration and single-use tokens
- **Audit Trail Implementation:** Comprehensive logging of professional contributions and data modifications
- **Real-time Collaboration:** Live updates when professionals complete their designated sections
- **Data Isolation:** Database design ensures professionals cannot access unauthorized application data

---

## Constraints & Assumptions

### Constraints

**Budget**
- **MVP Development:** Limited budget requiring cost-effective tech stack and minimal external services
- **Marketing Budget:** $20K allocated for customer acquisition (conferences, content marketing, referral programs)
- **Operating Costs:** Must maintain <25% COGS to achieve target 70%+ gross margins
- **Payment Processing:** 2.9% + $0.30 per transaction (Stripe standard pricing)

**Timeline**
- **Hard Deadline:** October 1, 2025 launch (25 days) - non-negotiable market opportunity
- **Development Sprint:** All MVP features must be complete and tested within 20 days (5 days buffer)
- **Legal/Compliance:** Minimal time available for complex regulatory review or legal opinion
- **User Testing:** Limited time for extensive user feedback and iteration

**Resources**
- **Development Team:** Small team familiar with Next.js, Tailwind, and Convex stack
- **Domain Expertise:** Limited in-house REAP program knowledge - requires external consultation
- **Customer Support:** Initially founder-led support with basic documentation
- **Sales/Marketing:** Founder-led initial customer acquisition and relationship building

**Technical**
- **AI Accuracy:** Template-based approach may limit application quality compared to advanced AI generation
- **Scaling Limitations:** MVP architecture must support 10x growth but may need refactoring for 100x
- **Integration Constraints:** Limited time for complex third-party integrations beyond core payment/AI services
- **Mobile Experience:** Web-responsive only for MVP - native apps deferred to Phase 2
- **Professional Delegation Complexity:** Granular permissions system adds significant technical complexity within timeline constraints

### Key Assumptions

**Market Assumptions**
- **REAP Program Reopening:** October 1st REAP FY 2026 opening proceeds as scheduled with no delays
- **Demand Surge:** Consultant workforce will pivot to commercial markets as residential tax credit expires
- **Pricing Acceptance:** $50 flat fee provides sufficient value proposition vs. $1,500-3,500 consultants
- **Application Quality:** Template-based AI generation will produce federally compliant applications with 80%+ approval rates
- **Professional Delegation Demand:** SME owners will actively use professional delegation features rather than handling applications independently

**Technical Assumptions**
- **AI API Reliability:** OpenAI/Claude APIs will maintain uptime and performance during high-usage periods
- **Convex Scaling:** Platform will handle October 1st traffic surge without performance degradation
- **Government API Availability:** USDA/federal databases for eligibility verification remain accessible
- **File Processing:** Standard business financial documents can be processed reliably for data extraction
- **Professional Delegation Security:** Convex can implement granular access controls securely within development timeline

**Business Model Assumptions**
- **Payment Conversion:** 95%+ of users who complete applications will pay the $50 fee
- **Customer Acquisition:** Industry conferences and direct outreach will yield 50+ installer company customers
- **User Retention:** 90%+ of consultants will continue using platform after initial successful applications
- **Viral Growth:** Satisfied installer companies will refer 2+ additional companies within 6 months
- **Professional Network Effects:** Delegated professionals will become repeat users across multiple SME clients

**Regulatory Assumptions**
- **Compliance Safety:** Template-based approach with human review will meet federal application requirements
- **Advocacy Compliance:** Minimal civic engagement reminders will not trigger regulatory scrutiny
- **Data Privacy:** Standard encryption and security practices sufficient for SME financial document handling
- **Payment Regulations:** Standard Stripe integration meets all financial service requirements
- **Professional Liability:** Platform audit trails provide sufficient protection for professional delegation relationships

**User Behavior Assumptions**
- **Document Availability:** SMEs will have required 3-year financials and energy usage data readily available
- **Technology Adoption:** Rural SME owners comfortable with web-based document upload and form completion
- **Consultant Willingness:** Solar consultants eager to adopt AI-assisted tools for competitive advantage
- **Manager Oversight:** Consultant managers will actively use dashboard features for team performance tracking
- **Professional Participation:** Accountants and advisors willing to work within third-party platform constraints
- **Trust in Delegation:** SME owners comfortable delegating sensitive financial data through secure invitation system

**Competitive Assumptions**
- **Market Entry Barriers:** 25-day development timeline creates first-mover advantage in REAP automation
- **Consultant Resistance:** Existing REAP consultants will not organize effective competitive response quickly
- **Technology Barriers:** Competitors will require 6+ months to develop comparable AI-powered platform
- **Price Competition:** $50 price point low enough to discourage competitive pricing wars
- **Professional Network Advantage:** First platform to market with professional delegation will capture network effects

**Professional Delegation Specific Assumptions**
- **Professional Willingness:** Accountants, engineers, and advisors will adopt platform workflows for client service
- **Security Acceptance:** Professionals comfortable with granular access controls limiting their data visibility
- **Client Trust:** SME owners trust platform security enough to invite external professionals
- **Workflow Integration:** Professional delegation enhances rather than complicates application processes
- **Revenue Opportunity:** Professional delegation creates additional revenue streams through network effects

---

## Risks & Open Questions

### Key Risks

**Timeline & Execution Risks**
- **25-Day Development Risk:** Unforeseen technical challenges could delay October 1st launch, missing critical market window
- **Professional Delegation Complexity:** Granular permissions and secure access controls may prove too complex for timeline constraints
- **AI Integration Complexity:** Template-based approach may prove insufficient for generating compliant federal applications
- **Quality Assurance Risk:** Limited testing time may result in bugs or compliance issues discovered post-launch
- **Team Capacity Risk:** Small development team may face burnout or capacity constraints during sprint

**Market & Competitive Risks**
- **REAP Program Delays:** USDA could postpone October 1st application opening, eliminating immediate market catalyst
- **Consultant Adoption Risk:** Solar consultants may resist AI-powered tools or prefer existing manual processes
- **Professional Delegation Adoption:** Accountants and advisors may resist platform-based client workflows
- **Price Sensitivity Risk:** $50 fee may be too high for smaller SMEs or too low to be perceived as valuable
- **Competitive Response Risk:** Existing REAP consultants could quickly lower prices or improve services to compete

**Technical & Operational Risks**
- **AI Reliability Risk:** OpenAI/Claude API outages or rate limits could prevent application generation during peak demand
- **Government System Integration:** USDA databases for eligibility verification may be unreliable or inaccessible
- **Data Security Risk:** Handling sensitive SME financial documents creates potential liability exposure
- **Professional Access Control Risk:** Granular permissions system may have security vulnerabilities or usability issues

**Regulatory & Compliance Risks**
- **Federal Application Compliance:** Template-generated applications may fail USDA review, damaging platform credibility
- **Professional Liability Risk:** Delegated professional relationships may create liability exposure not adequately covered by audit trails
- **Advocacy Feature Risk:** Even minimal civic engagement reminders could trigger unwanted regulatory attention
- **Data Privacy Risk:** Financial document handling may require compliance measures not yet implemented
- **Legal Liability Risk:** Incorrect applications could result in legal claims from affected SME businesses

**Business Model Risks**
- **Payment Conversion Risk:** Lower than expected payment rates could undermine revenue projections
- **Customer Acquisition Risk:** Difficulty reaching installer companies could limit user base growth
- **Professional Network Risk:** Delegated professionals may not create expected network effects or repeat usage
- **Retention Risk:** Poor initial user experience could prevent repeat usage and referrals
- **Market Size Risk:** Actual addressable market may be smaller than projected if eligibility is more restrictive

### Open Questions

**Product Development Questions**
- **AI Template Effectiveness:** Will template-based approach generate sufficiently high-quality applications for federal compliance?
- **Professional Delegation UI/UX:** What is the optimal user experience for inviting and managing professional contributors?
- **Document Processing:** Can standard OCR and data extraction reliably parse diverse SME financial document formats?
- **User Experience Flow:** What is the optimal user journey from document upload to final application submission?
- **Error Handling:** How should the platform handle incomplete or invalid document uploads from professionals?

**Market Validation Questions**
- **Consultant Willingness:** Are solar consultants genuinely interested in AI-assisted application tools?
- **Professional Adoption:** Will accountants and advisors embrace platform-based client service workflows?
- **SME Technology Adoption:** Will rural SME owners be comfortable with web-based document upload processes?
- **Professional Trust:** Will SME owners trust platform security enough to delegate sensitive financial data?
- **Pricing Optimization:** Is $50 the optimal price point, or should we test $25/$75 alternatives?
- **Geographic Distribution:** Which states/regions offer the highest concentration of qualified SMEs?

**Technical Architecture Questions**
- **Convex Professional Permissions:** Can Convex handle granular access controls for professional delegation securely and efficiently?
- **Real-time Performance:** Will application generation complete within the target <5 second timeframe?
- **Mobile Experience:** How critical is mobile optimization for consultant field usage and professional workflows?
- **Backup Systems:** What fallback options are needed if primary AI or payment systems fail?

**Business Operations Questions**
- **Customer Support:** What support volume should we expect, and how will we handle professional delegation technical issues?
- **Professional Onboarding:** How will we educate and onboard delegated professionals who aren't primary platform users?
- **Legal Requirements:** Do we need specific licenses or certifications to assist with federal grant applications?
- **Quality Assurance:** How will we validate that generated applications meet federal compliance standards?
- **Growth Strategy:** Should we prioritize installer company acquisition or direct SME customer acquisition?

**Regulatory & Compliance Questions**
- **REAP Program Changes:** Could USDA modify application requirements between now and October 1st?
- **Professional Liability Coverage:** What insurance coverage is needed for professional delegation relationships?
- **Advocacy Compliance:** What level of political engagement is legally permissible for platform users?
- **Data Retention:** How long must we retain SME financial documents, and what are deletion requirements?
- **Cross-Professional Compliance:** How do we ensure professional contributions meet their respective licensing requirements?

**Professional Delegation Specific Questions**
- **Professional Verification:** How will we verify credentials and qualifications of delegated professionals?
- **Liability Distribution:** How is professional liability distributed between platform, SME owner, and delegated professional?
- **Professional Pricing:** Should delegated professionals be able to charge additional fees through the platform?
- **Professional Relationship Management:** How will we manage ongoing relationships between SMEs and their delegated professionals?

### Areas Needing Further Research

**REAP Program Deep Dive**
- **Application Requirements:** Comprehensive analysis of all REAP FY 2026 application requirements and scoring criteria
- **Historical Success Rates:** Research on typical REAP application approval rates and common rejection reasons
- **Regional Variations:** Understanding of state-specific REAP implementation differences and requirements
- **Professional Requirements:** Research on whether specific professional credentials are required for application sections

**Competitive Intelligence**
- **Existing Solutions:** Analysis of current REAP consulting services and their methodologies
- **Professional Networks:** Identification of existing networks of rural energy professionals
- **Consultant Network Mapping:** Identification of key players and potential partnership opportunities
- **Technology Alternatives:** Research on existing grant application software and AI tools

**Legal & Regulatory Research**
- **Federal Compliance Requirements:** Legal review of requirements for software assisting with federal applications
- **Professional Liability Framework:** Understanding liability requirements for platform-facilitated professional services
- **Data Privacy Obligations:** Understanding of financial document handling requirements under federal and state law
- **Professional Licensing:** Research on cross-state professional licensing requirements for delegated services

**Market Research & Validation**
- **User Interviews:** Direct conversations with solar consultants, SME owners, and potential delegated professionals
- **Professional Market Research:** Survey of accountants, engineers, and advisors about platform-based client service interest
- **Installer Company Outreach:** Validation of interest level among target installer companies
- **Pilot Program Design:** Structure for limited beta testing with select customers before full launch

**Technical Feasibility Studies**
- **AI Quality Assessment:** Testing template-based approach against sample REAP applications
- **Security Penetration Testing:** Third-party security assessment of professional access control system
- **Professional Workflow Analysis:** Detailed analysis of how professionals currently handle similar client services

---

## Next Steps

### Immediate Actions (Next 7 Days)

1. **REAP Program Research & Compliance Analysis**
   - Download and analyze complete REAP FY 2026 application requirements and scoring criteria
   - Research historical approval rates and common rejection reasons 
   - Identify template structure for compliant application generation
   - Consult with REAP expert or experienced consultant for domain knowledge validation

2. **Technical Architecture Setup**
   - Initialize Next.js + Convex project repository with proper folder structure
   - Set up development environment with Tailwind CSS and TypeScript configuration
   - Configure Convex database schema for users, companies, applications, professional delegations, and file storage
   - Implement basic Convex Auth setup for multi-tenant user management

3. **Professional Delegation System Design**
   - Design database schema for granular professional access controls
   - Create magic link invitation system for professional onboarding
   - Develop audit trail system for tracking professional contributions
   - Design UI/UX for SME owners to invite and manage professional contributors

4. **AI Integration Prototype**
   - Create MVP application templates based on REAP requirements
   - Test OpenAI/Claude API integration for basic content generation
   - Develop document processing pipeline using Convex file storage
   - Validate template approach with sample SME financial data

5. **Market Validation & Legal Review**
   - Conduct 5+ interviews with solar consultants about current REAP pain points
   - Interview 3+ accountants/advisors about professional delegation interest
   - Contact 3+ installer companies to validate interest and pricing sensitivity
   - Consult legal counsel on grant application assistance requirements and professional liability

6. **Payment & Infrastructure Setup**
   - Configure Stripe integration for $50 application payments with flexible routing
   - Set up Resend for transactional email capabilities (magic links, professional invitations)
   - Deploy initial version to Vercel staging environment
   - Implement basic monitoring and error tracking

### Development Sprint (Days 8-20)

7. **Core Feature Implementation**
   - Build user registration and authentication flows for all user types (Account Admins, Consultants, SME owners, Professionals)
   - Develop guided application form with document upload capabilities
   - Implement professional delegation invitation and access control system
   - Build AI-powered application generation using template approach

8. **Professional Delegation Workflows**
   - Create secure professional invitation system with magic links
   - Implement granular access controls for professional data sections
   - Build professional-specific interfaces for section completion
   - Develop audit trail and tracking system for professional contributions

9. **Payment Processing & User Flows**
   - Complete Stripe payment integration for all customer types (installer companies, individual SMEs, professional-assisted applications)
   - Implement configurable payment routing logic managed by Account Admins
   - Build application review and submission confirmation flows
   - Add minimal civic engagement reminder feature

10. **Manager Dashboard & Company Controls**
    - Create basic manager dashboard for consultant oversight
    - Implement company-level application tracking and reporting
    - Build user management tools for Account Admins
    - Develop payment routing configuration interface

11. **Quality Assurance & Testing**
    - Conduct end-to-end testing with sample applications including professional delegation workflows
    - Validate generated applications against REAP compliance requirements
    - Load test platform for October 1st traffic surge scenarios
    - Test professional magic link security and access controls
    - Fix critical bugs and performance issues

### Launch Preparation (Days 21-25)

12. **Customer Acquisition Launch**
    - Create landing page with clear value proposition for installer companies
    - Develop professional delegation explanation and onboarding materials
    - Launch direct outreach campaign to target installer companies
    - Prepare for Solar Power International conference presence (if applicable)

13. **Documentation & Support Systems**
    - Create user documentation for all user types including professional delegation workflows
    - Develop FAQ addressing professional delegation security and liability questions
    - Set up customer support processes and escalation procedures
    - Prepare professional onboarding guidance and best practices

14. **Final Launch Preparation**
    - Deploy production version with monitoring and backup systems
    - Conduct final security review of professional access control system
    - Test payment processing for all customer types and routing scenarios
    - Prepare for October 1st REAP application surge with professional delegation workflows

### Post-Launch Actions (October-December 2025)

15. **Customer Success & Iteration**
    - Monitor application success rates and professional delegation usage patterns
    - Provide customer support for initial user onboarding including professional workflows
    - Gather feedback on professional delegation user experience and security
    - Iterate on professional invitation and access control systems based on real-world usage

16. **Professional Network Development**
    - Track professional adoption rates and repeat usage patterns
    - Identify opportunities for professional marketplace features
    - Analyze professional contribution quality and application success correlation
    - Develop professional success stories and case studies

17. **Growth & Expansion**
    - Scale customer acquisition based on initial success metrics
    - Begin planning Phase 2 features (professional marketplace, advanced AI)
    - Research expansion into additional grant programs leveraging professional network
    - Evaluate additional funding or partnership opportunities

18. **Performance Analysis & Optimization**
    - Analyze professional delegation impact on application approval rates
    - Track professional network effects and revenue implications
    - Optimize professional invitation and onboarding workflows
    - Prepare for Phase 2 development focused on professional services expansion

---

## PM Handoff

This Project Brief provides the full context for **reapSpring** - an AI-powered platform that automates REAP grant applications for the solar industry's commercial market transition, featuring a sophisticated professional delegation system that enables SME owners to leverage their existing professional relationships.

**Key Success Factors:**
- **October 1st launch is non-negotiable** - this is when REAP FY 2026 applications open
- **Professional delegation system** provides key competitive differentiation through secure, granular access controls
- **Template-based AI approach** balances quality with rapid development timeline while supporting professional contributions
- **Next.js + Convex + Stripe stack** leverages team familiarity for maximum velocity with built-in scaling capabilities
- **Multi-tenant architecture** serves installer companies → managers → consultants → SME clients with professional delegation
- **$50 pricing with flexible routing** disrupts traditional $1,500-3,500 consultant model while supporting various payment models

**Critical Next Steps:**
1. **REAP compliance research** - absolutely essential for generating valid applications
2. **Professional delegation system design** - core differentiator requiring careful security implementation  
3. **Legal review** - ensure platform meets federal application assistance and professional liability requirements  
4. **Customer validation** - confirm installer company and professional interest and pricing acceptance
5. **Technical execution** - 25-day sprint with professional delegation complexity but simplified coordination model

**Professional Delegation Implementation:**
- SME owners contact professionals directly and provide email addresses to platform
- Magic link system provides secure, time-limited access to specific data sections
- Independent professional workflows eliminate complex coordination requirements
- Audit trails maintain accountability and professional liability protection
- Granular access controls ensure professionals see only authorized data sections

**Post-MVP Vision:**
The platform expands from REAP-only to comprehensive grant application services across federal agencies, growing from $35M addressable market to $500M+ opportunity while building a sustainable professional services ecosystem and political advocacy infrastructure for program funding.

Please start in **PRD Generation Mode**, review this brief thoroughly, and work with the user to create the PRD section by section as the template indicates, asking for any necessary clarification or suggesting improvements.

---