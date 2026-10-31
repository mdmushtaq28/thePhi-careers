# ThePhi Careers & Workforce Platform

A responsive, dark premium frontend prototype for ThePhi's recruitment, agreement and workforce workflows.

## Run locally

No build step is required for this prototype.

1. Extract the ZIP.
2. Open `thephi-careers/index.html` in a browser.
3. For a local web server, run `python -m http.server 8000` from the `thephi-careers` folder and open `http://localhost:8000`.

## Included experience

- Premium public careers landing page and opportunity cards
- Five-step application flow with required-field checks and PDF resume validation
- Application confirmation and reference ID
- Applicant portal preview and application timeline
- Admin application table with search, filters, approve/reject demo actions
- Interview command center and sample scorecard
- Employee directory and onboarding checklist
- Recruitment analytics with illustrative charts and funnel metrics
- AI recruiter copilot interface with clearly labeled sample responses
- Agreement preview and physical fingerprint hardware-not-connected state
- Authorized representative signing desk preview
- Trust, privacy and security center
- Responsive layouts for desktop, tablet and mobile
- Browser-local persistence for demo application and admin status changes

## Important prototype limitations

This is a frontend prototype, not a production recruitment system. Sample dashboards and records are illustrative. Application submissions and admin status changes are stored only in the current browser's local storage. There is no real email delivery, account authentication, database, private file storage, AI provider connection, calendar integration, PDF signing, legal e-signature, or biometric scanner integration.

The fingerprint flow intentionally does not simulate a successful scan. A production integration needs a compatible physical scanner, its official SDK/API, an authenticated backend capture service, explicit informed consent, encrypted restricted storage, access auditing, and a reviewed retention/deletion policy. A browser cannot retrieve the fingerprint image from a phone or laptop's normal unlock sensor.

## Recommended production architecture

- Frontend: React, TypeScript, Vite, Tailwind CSS, accessible component system
- API: Node.js + Express with schema validation, rate limits, idempotency and structured errors
- Data: Supabase PostgreSQL with Row Level Security and migrations
- Identity: Supabase Auth, MFA for privileged users, role-based access control
- Documents: private Supabase Storage buckets, short-lived signed URLs, malware/file validation
- Notifications: configurable transactional email provider and in-app notification queue
- AI: server-side provider integration with permission-aware retrieval, explainable outputs and human review
- Agreements: versioned templates, immutable issued versions, server-side PDF rendering, SHA-256 integrity records and verified signing events
- Biometric hardware: replaceable provider adapter using the scanner manufacturer's official SDK/API
- Observability: error monitoring, audit events, backups, security alerts and operational metrics

## Production launch gates

1. Confirm ThePhi's legal entity details, policies, roles and agreement templates with qualified counsel.
2. Configure Supabase project, database migrations, RLS policies, Auth and private storage.
3. Implement and test every API endpoint and permission boundary.
4. Configure email domain authentication and notification templates.
5. Integrate a real signing provider or legally reviewed electronic-signature workflow.
6. Select and test compatible fingerprint hardware. Do not collect biometrics until consent, lawful basis, security, retention and deletion are approved.
7. Add automated tests, accessibility checks, security review, backups and incident response.
8. Deploy frontend and API with HTTPS, secrets management and monitoring.

## Design direction

Premium technology-company aesthetic: deep navy surfaces, restrained lime and cyan accents, high-contrast typography, subtle gradients, clear hierarchy, responsive cards, concise data displays and explicit status labels.
