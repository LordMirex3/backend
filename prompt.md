---
mode: Beastmode
---
# MyTypist Backend Documentation

## Overview

MyTypist (mytypist.net) is a comprehensive document automation SaaS platform for Nigerian businesses. It enables users to create, customize, and generate professional documents using intelligent template processing with placeholder detection and replacement. The platform supports both pay-as-you-go and subscription-based billing models, integrated with Flutterwave for seamless Nigerian payment processing.

## Core Features

### 1. Document Management
- Document Creation & Generation
  - Template-based document generation
  - Placeholder detection and replacement
  - Multi-format support (DOCX, PDF)
  - Real-time preview
  - Document sharing and collaboration
  - Version control
  - Document history and audit trails

### 2. User Management & Authentication
- User System
  - Role-based access control (Admin, Moderator, User, Guest)
  - User profiles and preferences
  - Activity tracking
  - Session management
- Authentication
  - JWT-based authentication
  - Password security
  - Multi-factor authentication
  - Session management

### 3. Payment & Billing
- Payment Processing
  - Flutterwave integration
  - Token system
  - Subscription management
  - Pay-as-you-go billing
  - Payment history
- Token System
  - Token purchase
  - Usage tracking
  - Balance management
  - Auto-renewal

### 4. Template System
- Template Management
  - Template creation and editing
  - Category management
  - Version control
  - Preview generation
- Template Marketplace
  - Pricing controls
  - User submissions
  - Revenue sharing
  - Usage analytics

### 5. Notification System
- Notification Types
  - In-app notifications
  - Email notifications
  - System alerts
- Notification Management
  - Delivery tracking
  - Custom preferences
  - Template-based notifications

### 6. Analytics & Reporting
- Usage Analytics
  - User metrics
  - Document metrics
  - Revenue tracking
  - Performance monitoring
- Audit System
  - Security logging
  - Activity tracking
  - Compliance reporting
  - Error tracking

### 7. Growth & Engagement
- SEO Optimization
  - Meta tags
  - OpenGraph data
  - Sitemap generation
- Referral System
  - Partner program
  - Revenue sharing
  - Performance tracking
  - Analytics dashboard

## Current Development Status

### 1. Landing Page & Guest Document Generation
- [x] Template Search & Preview
  - [x] Real-time search with autocomplete (enhanced with caching)
  - [x] Preview templates without login (secure watermarked PDFs)
  - [x] Popular/recent templates display (with analytics)
  - [x] SEO-optimized template pages (meta tags, OpenGraph)

- [x] Guest Document Creation
  - [x] Create document without login (with fraud prevention)
  - [x] Auto-save inputs for suggestions (with smart validation)
  - [x] Live preview as user types (with responsive thumbnails)
  - [x] Registration prompt for download (with security checks)
  - [x] Auto-link document to new user account (with enhanced tracking)

### 2. Template Management & Preview
- [x] Admin Template Management
  - [x] Upload preview & extraction files
  - [x] Set metadata (title, desc, tags)
  - [x] Manage categories and groups
  - [x] Version control & history

- [x] Pricing Controls
  - [x] Set individual template prices
  - [x] Bulk pricing updates
  - [x] Category/tag-based pricing
  - [x] Special offers/discounts

- [x] User Template Submissions
  - [x] Submit templates for review
  - [x] Admin approval workflow
  - [x] Public/private settings
  - [x] Usage tracking & revenue sharing

### 3. Admin Dashboard & Analytics
- [x] Real-time Statistics
  - [x] User metrics (active, new, total)
  - [x] Document metrics (created, downloaded)
  - [x] Revenue tracking
  - [x] Visit analytics (per page, duration)

- [x] Data Management
  - [x] Export data (CSV, PDF, Excel)
  - [x] Visualization APIs for charts
  - [x] Custom date ranges
  - [x] Trend analysis

- [x] Audit System
  - [x] Complete activity logs with advanced threat detection
    - [x] SQL injection detection
    - [x] XSS attack detection
    - [x] Rate limiting patterns
    - [x] Suspicious IP tracking
    - [x] Unusual behavior detection
    - [x] Account takeover prevention
  - [x] Security audit trail
    - [x] Detailed incident tracking
    - [x] Geographic data
    - [x] Attack pattern analysis
    - [x] Evidence collection
  - [x] Admin action tracking
    - [x] Response time monitoring
    - [x] Resolution tracking
    - [x] Investigation notes
    - [x] Mitigation steps
  - [x] Data compliance reports
    - [x] Incident summaries
    - [x] Pattern analysis
    - [x] Response metrics
    - [x] Geographic data analysis

### 4. User & Role Management
- [x] Role-Based Access Control
  - [x] Admin (full access)
  - [x] Moderator (limited access)
  - [x] User (standard access)
  - [x] Guest (preview access)

- [x] User Management
  - [x] Create/edit/suspend users (implemented in admin.py)
  - [x] Bulk actions (implemented in admin.py)
  - [x] Plan assignment (implemented in admin.py)
  - [x] Usage monitoring (implemented in admin.py)

- [x] Moderator System
  - [x] Create moderator accounts (implemented in moderator_management.py)
  - [x] Define permissions (implemented in role_management.py)
  - [x] Activity tracking (implemented with AuditService)
  - [x] Support tools (integrated with SupportTicketService)

### 5. Document Sharing & Version Control
- [x] Public Document Sharing
  - [x] SEO-optimized public document links
  - [x] No authentication required for viewing
  - [x] Original view for downloaded documents (no watermark)
  - [x] Watermarked previews for public templates
  - [x] View tracking and analytics
    - [x] Total views and unique visitors
    - [x] Traffic sources and referrers
    - [x] Geographic data and device info
    - [x] GDPR-compliant tracking
  - [x] Conversion tracking (views to downloads)
 

### 6. SEO & Social Integration
- [x] SEO Optimization
  - [x] Meta tags generation (implemented in SEOService)
  - [x] OpenGraph data (dynamic generation based on content)
  - [x] Canonical URLs (middleware and URL service)
  - [x] Sitemap generation (XML sitemap with priority)

- [x] Social Sharing
  - [x] Share previews (dynamic image generation)
  - [x] Social media cards (custom preview for each platform)
  - [x] Engagement tracking (comprehensive analytics)
  - [x] Viral sharing features (QR codes and tracking)

### 7. Referal



- [ ] Partnership System
  - [x] Partner applications
  - [x] Revenue sharing
  - [x] Performance tracking
  - [x] Partner dashboard

### 8. Advanced Features
- [x] Notifications
  - [x] In-app notifications
  - [x] Email notifications
  - [x] Custom preferences

- [x] Token System
  - [x] Token purchase
  - [x] Usage tracking
  - [x] Auto-renewal
  - [x] Balance alerts

- [x] Performance
  - [x] Response time < 500ms
  - [x] Caching strategy
  - [x] Load balancing
  - [x] Auto-scaling

## User Preferences

Preferred communication style: Simple, everyday language.

CRITICAL: Never duplicate existing code or create new files that replicate functionality that already exists. Instead, always check for existing files and functionality first, and extend or modify those files as needed. When implementing new features or making updates, search the entire codebase to find relevant existing code that can be reused or extended. This applies to all code changes including routes, services, models, and utilities.

The agent should continuously read and analyze the entire codebase to detect changes. When changes are identified, the agent should analyze the existing code patterns, architectural decisions, coding style, and implementation approaches. It should think exactly like the original developer, ensuring that any modifications strictly follow the established coding patterns and practices already present in the codebase. It should not introduce new coding approaches, patterns, or styles that deviate from what has already been implemented, and if a deviation is needed, it should ask for permission.

The agent must thoroughly analyze the existing codebase before making any changes to understand the established patterns. It must pay attention to naming conventions, error handling approaches, data structure usage, and architectural patterns already in use. It must consider the existing code organization, module structure, and dependency management approaches. It must evaluate the current testing patterns, logging approaches, and configuration management styles. It should only update files when there is a clear necessity, not for cosmetic or preference-based changes. It should update the context of this file after each feature completion and update this replit.md file when new patterns or rules are discovered during development. It must follow DRY (Don't Repeat Yourself) principles – eliminating duplicate code, commits, and object instantiation. It must ensure database migrations match model declarations (column names, nullable fields, foreign keys) and proactively check and update related files when making changes – not waiting to be told. After every feature completion, it should analyze and remove unused imports and dead code. It should provide a concise summary after each feature: group methods/functions under each file created/modified, with a one-sentence purpose. It must update the Application Summary section at the end of this file when new features or major functionality are implemented. The agent's life depends on maintaining absolute consistency with the existing codebase patterns and never introducing foreign coding approaches that conflict with the established development style.

## Recent Feature/Refactor Summary

### app/tasks/document_tasks.py
- `generate_document_thumbnail`: Now uses Pillow, pdf2image, and docx2pdf to generate real thumbnails for DOCX, PDF, and image files. Removed all placeholder logic and comments.

### app/tasks/payment_tasks.py
- `send_payment_success_notification`, `send_payment_failure_notification`, `send_subscription_renewal_notification`: Now use the real EmailService to send notifications (SendGrid/SMTP), removed all print/log-only and placeholder logic.

All placeholder, "for now", and TODO comments in these modules have been removed. All notification and thumbnail logic is now production-grade.

## System Architecture

The backend is built on **FastAPI** for high performance, async support, and automatic API documentation. It achieves sub-500ms document generation and <50ms API response times.

**PostgreSQL** is the primary database, chosen for production-grade performance, scalability, and robust ACID compliance, with advanced connection pooling and query optimization.

**Redis** serves as both a caching layer and message broker for background tasks. **Celery** handles asynchronous operations like document generation and payment processing to maintain API responsiveness.

The document processing system uses a template-based approach with intelligent placeholder detection. DOCX files with `{variable_name}` placeholders are uploaded. Real-time placeholder extraction uses `python-docx`. Background generation is handled by Celery, supporting complex formatting and multiple file formats. Placeholder logic handles dynamic sizing and positioning for text, dates, images, and signatures, including features like intelligent input forms, date formatting, and image/signature placement. The system intelligently saves past user inputs for autocomplete and suggestions. The admin can customize placeholder behavior (e.g., input type, optional/required status, formatting).

Multi-layered security includes **JWT-based authentication**, **rate limiting middleware** (Redis-backed), **security headers middleware** (XSS, CSRF, clickjacking), **audit logging**, and **input validation** using Pydantic schemas.

**Flutterwave integration** is optimized for the Nigerian market, supporting local payment methods, webhook verification, subscription management, and a balance system for pay-as-you-go users.

Role-based access control supports **Standard users**, **Admin users**, and **Guest users**. Admin users manage system settings, users, and templates. Guest users have limited access for free document creation and preview, requiring registration for download. Users registering through the main page can choose pay-as-you-go or subscription plans. Admins configure token values, document prices, minimum/maximum deposits, trial credits, and subscription plan details. The system handles free trials, token deductions, insufficient token notifications, and subscription renewals with grace periods and credit transfers.

The system features an organized file storage for templates, generated documents, and user uploads, with SHA256 integrity verification and automatic cleanup.

The API design is RESTful, with modular routes, consistent error handling, request/response validation, automatic OpenAPI documentation, and CORS configuration. Performance is optimized through database connection pooling, background task processing, Redis caching, and efficient file handling.

Moderator accounts are created by admins, who define roles and permissions (e.g., reviewer, support, analytics, tester). Moderators have tailored dashboards based on their assigned permissions. The system tracks moderator activity for payment purposes. Account creation triggers an email notification, with an immediate password change encouraged upon first login.

## External Dependencies

# Development Guidelines

## Code Organization and Updates

1. NO CODE DUPLICATION: Never create new files that replicate functionality that already exists in the codebase. Always:
   - Search the entire codebase for existing implementations
   - Analyze existing files and functionality first
   - Extend or modify existing files instead of creating new ones
   - Look for reusable code in routes, services, models, and utilities
   - Avoid creating new patterns when existing ones can be reused

2. Update Process:
   - Read the entire codebase to understand existing patterns
   - Search for files that handle similar functionality
   - Modify existing files to add new features
   - Maintain consistent patterns and approaches
   - Document any changes in this file

## External Dependencies

### Core Framework Dependencies
- **FastAPI**: Web framework
- **SQLAlchemy**: Database ORM
- **Alembic**: Database migration management
- **Pydantic**: Data validation and settings management

### Authentication and Security
- **PyJWT**: JSON Web Token
- **Passlib**: Password hashing
- **Python-multipart**: File upload handling

### Database and Caching
- **PostgreSQL**: Primary database
- **Redis**: Caching and message broker
- **Celery**: Distributed task queue

### Document Processing
- **python-docx**: DOCX manipulation
- **PyPDF2**: PDF processing
- **Pillow**: Image processing

### Payment Processing
- **Flutterwave Python SDK**: Payment gateway integration
- **Requests**: HTTP client
- **HMAC**: Webhook signature verification

### Background Tasks and Scheduling
- **Celery**: Asynchronous task processing
- **Redis**: Message broker/result backend for Celery
- **APScheduler**: Advanced Python scheduler

### Development and Monitoring
- **Uvicorn**: ASGI server
- **Python-dotenv**: Environment variable management
- **Sentry**: Error tracking and performance monitoring

### Email and Communication
- **Sendgrid/SMTP**: Email service integration
- **Jinja2**: Template engine

### API Documentation and Testing
- **Swagger/OpenAPI**: Automatic API documentation
- **Pytest**: Testing framework
- **HTTPX**: Async HTTP client for testing

## Code Cleanup & Organization Checklist

### 1. Route Standardization
- [ ] Standardize all routes to use consistent /api prefix
- [ ] Remove version prefixes (v1, v2, etc.)
- [ ] Clean up route naming (remove enhanced, advanced, etc.)
- [ ] Organize route groups logically
- [ ] Update OpenAPI documentation

### 2. File Organization
- [ ] Identify and remove duplicate files
- [ ] Consolidate similar functionalities
- [ ] Standardize file naming conventions
- [ ] Create proper module hierarchy
- [ ] Update import statements

### 3. Code Cleanup
- [ ] Remove unused imports
- [ ] Clean up commented code
- [ ] Fix inconsistent naming
- [ ] Standardize error handling
- [ ] Update type hints

### 4. Service Layer
- [ ] Consolidate duplicate services
- [ ] Standardize service naming
- [ ] Fix circular dependencies
- [ ] Improve error handling
- [ ] Add missing documentation

### 5. Database & Models
- [ ] Review and update migrations
- [ ] Fix model relationships
- [ ] Standardize model naming
- [ ] Add missing indexes
- [ ] Update field constraints

### 6. Testing & Validation
- [ ] Fix broken tests
- [ ] Add missing tests
- [ ] Update validation schemas
- [ ] Test all routes
- [ ] Verify dependencies

## Agent progress

- [x] Remove dev placeholders — MockRedis fallback made config-controlled and misleading startup prints reduced. See `main.py` and `config.py` for SKIP_DB_TABLE_CREATION and REDIS_ENABLED flags.