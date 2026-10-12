<<<<<<< HEAD
<a href="https://demo-nextjs-with-supabase.vercel.app/">
  <img alt="Next.js and Supabase Starter Kit - the fastest way to build apps with Next.js and Supabase" src="https://demo-nextjs-with-supabase.vercel.app/opengraph-image.png">
  <h1 align="center">Next.js and Supabase Starter Kit</h1>
</a>

<p align="center">
 The fastest way to build apps with Next.js and Supabase
</p>

<p align="center">
  <a href="#features"><strong>Features</strong></a> ·
  <a href="#demo"><strong>Demo</strong></a> ·
  <a href="#deploy-to-vercel"><strong>Deploy to Vercel</strong></a> ·
  <a href="#clone-and-run-locally"><strong>Clone and run locally</strong></a> ·
  <a href="#feedback-and-issues"><strong>Feedback and issues</strong></a>
  <a href="#more-supabase-examples"><strong>More Examples</strong></a>
</p>
<br/>

## Features

- Works across the entire [Next.js](https://nextjs.org) stack
  - App Router
  - Pages Router
  - Proxy
  - Client
  - Server
  - It just works!
- supabase-ssr. A package to configure Supabase Auth to use cookies
- Password-based authentication block installed via the [Supabase UI Library](https://supabase.com/ui/docs/nextjs/password-based-auth)
- Styling with [Tailwind CSS](https://tailwindcss.com)
- Components with [shadcn/ui](https://ui.shadcn.com/)
- Optional deployment with [Supabase Vercel Integration and Vercel deploy](#deploy-your-own)
  - Environment variables automatically assigned to Vercel project

## Demo

You can view a fully working demo at [demo-nextjs-with-supabase.vercel.app](https://demo-nextjs-with-supabase.vercel.app/).

## Deploy to Vercel

Vercel deployment will guide you through creating a Supabase account and project.

After installation of the Supabase integration, all relevant environment variables will be assigned to the project so the deployment is fully functioning.

[![Deploy with Vercel](https://vercel.com/button)](https://vercel.com/new/clone?repository-url=https%3A%2F%2Fgithub.com%2Fvercel%2Fnext.js%2Ftree%2Fcanary%2Fexamples%2Fwith-supabase&project-name=nextjs-with-supabase&repository-name=nextjs-with-supabase&demo-title=nextjs-with-supabase&demo-description=This+starter+configures+Supabase+Auth+to+use+cookies%2C+making+the+user%27s+session+available+throughout+the+entire+Next.js+app+-+Client+Components%2C+Server+Components%2C+Route+Handlers%2C+Server+Actions+and+Middleware.&demo-url=https%3A%2F%2Fdemo-nextjs-with-supabase.vercel.app%2F&external-id=https%3A%2F%2Fgithub.com%2Fvercel%2Fnext.js%2Ftree%2Fcanary%2Fexamples%2Fwith-supabase&demo-image=https%3A%2F%2Fdemo-nextjs-with-supabase.vercel.app%2Fopengraph-image.png)

The above will also clone the Starter kit to your GitHub, you can clone that locally and develop locally.

If you wish to just develop locally and not deploy to Vercel, [follow the steps below](#clone-and-run-locally).

## Clone and run locally

1. You'll first need a Supabase project which can be made [via the Supabase dashboard](https://database.new)

2. Create a Next.js app using the Supabase Starter template npx command

   ```bash
   npx create-next-app --example with-supabase with-supabase-app
   ```

   ```bash
   yarn create next-app --example with-supabase with-supabase-app
   ```

   ```bash
   pnpm create next-app --example with-supabase with-supabase-app
   ```

3. Use `cd` to change into the app's directory

   ```bash
   cd with-supabase-app
   ```

4. Rename `.env.example` to `.env.local` and update the following:

  ```env
  NEXT_PUBLIC_SUPABASE_URL=[INSERT SUPABASE PROJECT URL]
  NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY=[INSERT SUPABASE PROJECT API PUBLISHABLE OR ANON KEY]
  ```
  > [!NOTE]
  > This example uses `NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY`, which refers to Supabase's new **publishable** key format.
  > Both legacy **anon** keys and new **publishable** keys can be used with this variable name during the transition period. Supabase's dashboard may show `NEXT_PUBLIC_SUPABASE_ANON_KEY`; its value can be used in this example.
  > See the [full announcement](https://github.com/orgs/supabase/discussions/29260) for more information.

  Both `NEXT_PUBLIC_SUPABASE_URL` and `NEXT_PUBLIC_SUPABASE_PUBLISHABLE_KEY` can be found in [your Supabase project's API settings](https://supabase.com/dashboard/project/_?showConnect=true)

5. You can now run the Next.js local development server:

   ```bash
   npm run dev
   ```

   The starter kit should now be running on [localhost:3000](http://localhost:3000/).

6. This template comes with the default shadcn/ui style initialized. If you instead want other ui.shadcn styles, delete `components.json` and [re-install shadcn/ui](https://ui.shadcn.com/docs/installation/next)

> Check out [the docs for Local Development](https://supabase.com/docs/guides/getting-started/local-development) to also run Supabase locally.

## Feedback and issues

Please file feedback and issues over on the [Supabase GitHub org](https://github.com/supabase/supabase/issues/new/choose).

## More Supabase examples

- [Next.js Subscription Payments Starter](https://github.com/vercel/nextjs-subscription-payments)
- [Cookie-based Auth and the Next.js 13 App Router (free course)](https://youtube.com/playlist?list=PL5S4mPUpp4OtMhpnp93EFSo42iQ40XjbF)
- [Supabase Auth and the Next.js App Router](https://github.com/supabase/supabase/tree/master/examples/auth/nextjs)
=======
# Product Specification: Incident Reporting & Public Accountability Platform

**Working title:** Ngori Report 
**Initial institutional client:** Police department (simulated for the MVP)  
**Initial market:** Kenya  
**Product stage:** MVP / hackathon prototype  
**Product type:** Web-based incident reporting and case accountability system

## 1. Problem Statement

Citizens need a structured way to report incidents, submit relevant information, and track the handling of their reports. Where existing reporting processes do not provide accessible progress updates or clear records of actions taken, reporters may struggle to understand the status of their cases and hold responsible institutions accountable.

The proposed platform provides a centralized digital workflow for submitting incident reports, managing their progress, recording actions taken, and generating accountability information.

The platform will use AI to assist with incident classification, identification of potentially relevant legal provisions, detection of missing information, and comparison of recorded case progress against applicable procedural guidance.

**Core problem:** How can incident reporting become more traceable, accessible, and accountable from submission through resolution?

**Product objective:** Demonstrate an end-to-end reporting and tracking workflow that improves visibility into case handling while protecting sensitive information.

## 2. Target Users

### Primary users

**A. Citizens / Reporters**
- Submit incident reports.
- Receive a unique reference number.
- View permitted updates on their reports.
- Provide additional information and upload authorized documents.
- Receive notifications when their cases change status.
- Submit feedback on the handling of their reports.

**B. Case-handling officers**
- View reports assigned to them.
- Review incident details and authorized attachments.
- Assess AI-generated classifications and legal references.
- Update case status and record actions taken.
- Request additional information from reporters.
- Record outcomes and reasons for closure.

**C. Supervisors / Institutional administrators**
- Assign and reassign cases.
- Monitor workload and overdue cases.
- Review case histories and escalations.
- Monitor aggregate performance indicators.
- Audit actions taken by authorized users.

### Secondary users

**D. Public / Community members**
- View explicitly published, non-sensitive institutional reports and aggregate statistics.
- Raise public-interest issues in a future release.
- Comment on published issues and official responses where enabled.

**Initial scope decision:** The MVP will prioritize individual incident reporting and case tracking. Public civic issues and community discussions will be deferred until the private case-management workflow works reliably.

## 3. Core Workflow

### A. Incident reporting

1. A reporter creates an account or uses an approved reporting method.
2. The reporter selects an incident category and provides the required details.
3. The system validates required fields and identifies missing information.
4. The reporter submits the report.
5. The system generates a unique case reference and records the submission time.
6. The reporter receives confirmation that the report has been received.

### B. Verification and review

1. The system records the account's verification status.
2. An authorized officer reviews the submitted information.
3. The officer records whether the report is accepted for processing, requires additional information, or is referred elsewhere.
4. Any verification decision is recorded with its timestamp and responsible user.
5. AI-generated classifications remain advisory until reviewed by an authorized person.

Account verification does not automatically establish the truth of an allegation. Likewise, an unverified report is not necessarily a false report.

### C. Case handling and progress tracking

1. An authorized supervisor assigns the case to a responsible officer or unit.
2. The assigned officer reviews the report and records actions taken.
3. Each status change creates a timestamped history entry.
4. The reporter views updates permitted for their role.
5. The reporter may provide additional information or permitted documents.
6. Cases that exceed configured handling intervals are flagged for review.
7. An authorized officer records the outcome and closure reason.
8. The reporter may submit feedback on the handling of the case.

### D. AI-assisted analysis

1. The system analyzes the incident description and available structured fields.
2. It suggests an incident category and potentially relevant legal provisions.
3. It identifies missing information and possible next procedural steps.
4. It compares recorded progress with applicable procedural guidance, where a reliable reference exists.
5. It generates a structured summary with supporting sources, limitations, and items requiring human review.
6. Authorized users review the analysis and record any corrections or decisions.

### E. Public accountability

For the MVP, the platform will display aggregate statistics derived from demonstration data. It will not expose individual case files or sensitive evidence through the public dashboard.

Public civic issue submissions, community comments, and official public responses will be considered in a later release.

## 4. MVP Features

The MVP will implement one complete workflow rather than several incomplete modules.

### Feature 1: Incident submission
- Reporter account creation and login.
- Incident category, description, date, and location fields.
- Optional contact information and permitted attachments.
- Required-field validation.
- Unique case reference generation.
- Submission confirmation.

### Feature 2: Case tracking
- Case list and case-detail view for the reporter.
- Defined case statuses.
- Timestamped status history.
- Officer progress updates.
- Additional-information requests.
- Reporter feedback at closure.

### Feature 3: Officer dashboard
- Secure officer login.
- Queue of submitted and assigned cases.
- Case review and assignment.
- Status updates and action notes.
- Access-controlled document viewing.
- Case closure with an outcome and reason.

### Feature 4: AI-assisted case analysis
- Suggested incident classification.
- Retrieval of relevant passages from a limited, verified legal knowledge base.
- Identification of missing information.
- Suggested procedural actions for human review.
- Comparison of recorded progress against applicable procedural guidance.
- Structured analysis report containing citations, limitations, and review status.

### Feature 5: Audit trail
- Record of case creation and status changes.
- Record of assignment and reassignment.
- Record of document uploads and access-sensitive actions.
- Record of AI-generated assessments and subsequent human corrections.
- Attribution of actions to authenticated users.

### Feature 6: Public accountability dashboard
- Aggregate case counts by category and status.
- Demonstration response-time and resolution-time statistics.
- Clear distinction between live operational data and synthetic demo data.
- No public access to raw evidence or restricted case details.

### MVP acceptance criterion

A reporter can submit a case, receive a reference number, and view its progress; an officer can review and update the case; the AI can produce a source-grounded assessment; and the public dashboard can display aggregate statistics without exposing restricted information.

## 5. Explicitly Excluded Features

The following will not be implemented in the first version:

- Direct integration with live police databases or dispatch systems.
- Automated arrest, prosecution, guilt, or legal-liability decisions.
- Automatic determination that a complaint or piece of evidence is truthful.
- Biometric verification, facial recognition, or automated identity-document verification.
- Public browsing of individual police reports or case evidence.
- Nationwide deployment or integrations across multiple government agencies.
- Native Android or iOS applications.
- Blockchain-based evidence storage or case tracking.
- Automated emergency dispatch or emergency-response guarantees.
- Public comments on confidential cases.
- Automated legal representation or definitive legal advice.
- Production use with real sensitive case data before appropriate security, legal, and institutional reviews.

The MVP is not an emergency-reporting channel. Its interface must clearly direct users facing immediate danger to appropriate established emergency services.

## 6. User Roles and Permissions

### Reporter
- Create and submit reports.
- View their own reports and permitted status updates.
- Upload permitted additional information.
- View feedback requests and submit feedback.
- Cannot assign cases, edit official case records, or view other reporters' cases.

### Case officer
- View cases assigned to them or otherwise explicitly authorized.
- Review relevant case details and attachments.
- Add progress updates and request information.
- Review AI analysis and record corrections.
- Cannot change system-wide permissions or access unrelated restricted cases without authorization.

### Supervisor / administrator
- Assign cases and manage officer workloads.
- Review escalations and case histories.
- Manage authorized users and role assignments.
- Access aggregate operational reports.
- Perform only those case-access and administrative actions permitted by the institutional policy.

### Public visitor
- View approved public information and aggregate statistics.
- Cannot view confidential case information or raw evidence.
- May access public civic issue features when these are introduced.

**Important:** Administrative privileges must not automatically imply unrestricted access to every document. Sensitive information should be protected through explicit permissions and audit logging.

## 7. Initial Data Model

The initial relational database will contain the following entities.

### Users
- `id`
- `name`
- `email`
- `role`
- `account_status`
- `verification_status`
- `created_at`

### Cases
- `id`
- `reference_number`
- `reporter_id`
- `category`
- `description`
- `incident_datetime`
- `location`
- `status`
- `priority`
- `created_at`
- `closed_at`

### Case Assignments
- `id`
- `case_id`
- `assigned_to`
- `assigned_by`
- `assigned_at`
- `ended_at`

### Case Status History
- `id`
- `case_id`
- `previous_status`
- `new_status`
- `changed_by`
- `public_update`
- `internal_note`
- `created_at`

### Case Documents
- `id`
- `case_id`
- `uploaded_by`
- `storage_key`
- `file_hash`
- `document_classification`
- `access_level`
- `created_at`

### AI Assessments
- `id`
- `case_id`
- `model_version`
- `suggested_category`
- `legal_references`
- `missing_information`
- `suggested_actions`
- `progress_assessment`
- `limitations`
- `review_status`
- `created_at`

### Audit Events
- `id`
- `actor_id`
- `case_id`
- `action`
- `target_type`
- `target_id`
- `created_at`

### Case Outcomes
- `id`
- `case_id`
- `outcome_category`
- `closure_reason`
- `recorded_by`
- `created_at`

### Reporter Feedback
- `id`
- `case_id`
- `reporter_id`
- `rating`
- `feedback`
- `created_at`

The database may evolve as requirements become clearer. Access controls, relationships, validation rules, and data-retention requirements must be designed alongside the schema rather than added as an afterthought.

## 8. AI Responsibilities and Limitations

### AI responsibilities

1. **Classification:** Suggest a category and subcategory from the supplied incident details.
2. **Legal information retrieval:** Retrieve potentially relevant provisions from an approved Kenyan legal knowledge base.
3. **Information-gap detection:** Identify missing facts that may be necessary for an authorized reviewer.
4. **Procedural assistance:** Suggest possible next steps based on documented procedures.
5. **Progress comparison:** Compare recorded actions with applicable procedural or remedial guidance, flagging apparent gaps.
6. **Report generation:** Produce a structured summary of the incident, recorded actions, outstanding information, and current status.

### AI requirements

- Legal claims must be linked to identifiable source documents and relevant provisions.
- The system must distinguish verified source text from AI-generated interpretation.
- The AI must indicate when available information is insufficient.
- Recommendations must remain advisory.
- Authorized human reviewers must be able to correct or reject AI suggestions.
- The system must retain the assessment and its model/version metadata for auditing.
- The AI must not invent legal provisions, procedural requirements, case updates, or evidence.
- The AI must not independently publish sensitive case information.

### Legal knowledge base

The initial knowledge base will cover a limited set of incident categories using verified Kenyan constitutional provisions, relevant legislation, and authoritative procedural guidance.

Each source should include its title, issuing authority, publication or revision date where available, relevant section, and source URL.

The knowledge base must be reviewed for currency and applicability. Retrieval from a source does not itself establish that a particular legal provision applies to an individual case.

## 9. Security and Privacy Assumptions

The platform may process personal information, allegations of criminal conduct, witness details, and potentially sensitive evidence. The prototype must therefore be designed with a clear separation between demonstration functionality and production readiness.

### MVP requirements
- Use synthetic data for public demonstrations.
- Apply role-based access controls on the server, not only in the interface.
- Require authentication for restricted case information.
- Store uploaded documents in private storage with controlled access.
- Validate uploads and restrict allowed file types and sizes.
- Avoid placing sensitive information in public URLs, application logs, or AI prompts unnecessarily.
- Use secure transport and appropriately protected secrets.
- Record important case-management and administrative actions.
- Separate internal notes from reporter-visible updates.
- Prevent public dashboards from exposing identifiable case information.
- Establish basic backup, recovery, and data-retention procedures.

### Before production deployment
- Conduct a privacy impact assessment where required.
- Review compliance with Kenya's Data Protection Act, 2019, and applicable regulations.
- Establish a lawful basis for processing, appropriate notices, and data-subject rights procedures.
- Define retention, deletion, access, disclosure, and incident-response policies.
- Assess the security of the AI provider and the handling of submitted data.
- Establish institutional authorization, access policies, and operational responsibilities.
- Conduct independent security testing and obtain appropriate legal review.
- Establish procedures for correcting inaccurate records and handling malicious or abusive submissions.

Identity verification, allegation verification, and evidence authenticity are separate processes. The platform must not treat any one of them as proof of the others.

## 10. Success Metrics

The MVP will be evaluated on whether it completes the intended workflow, produces useful AI assistance, and protects information appropriately.

### Functional metrics
- At least 95% of valid test submissions create a case successfully.
- 100% of successfully created test cases receive unique reference numbers.
- 100% of tested status changes appear in the case history with the correct actor and timestamp.
- All tested role-permission scenarios behave as specified.
- All tested restricted-document access attempts are denied to unauthorized users.
- One demonstration case completes the full workflow from submission to recorded resolution.

### AI quality metrics
- Classification performance is evaluated against a manually labelled test set.
- Legal references are checked against the approved source material.
- Unsupported legal citations are treated as critical failures.
- Missing-information suggestions are evaluated by a human reviewer.
- Progress assessments are checked against predefined test scenarios.
- AI-generated assessments are distinguishable from verified case facts and official decisions.

Targets for classification accuracy and other AI performance measures must be set after creating a representative test set; they should not be invented before evaluation.

### Usability metrics
- At least 80% of test users can submit a report without assistance.
- At least 80% of test users can locate a case and understand its current status.
- Test users can distinguish public updates from confidential internal notes.

### Accountability metrics
- Every tested case assignment, status change, and closure has an attributable record.
- The dashboard's aggregate statistics reconcile with the underlying test data.
- Overdue cases can be identified using configurable rules.
- Every displayed performance metric has a defined calculation method.

### Demo acceptance test

A successful MVP demonstration must show:

1. A citizen submits a synthetic incident.
2. The platform generates a reference number.
3. The AI produces a structured assessment with traceable legal references.
4. An officer reviews and assigns the case.
5. The officer records an action and updates the status.
6. The citizen sees the permitted progress update.
7. The case is closed with a recorded outcome.
8. The public dashboard updates its aggregate statistics without exposing restricted information.

**Definition of success:** A working, testable end-to-end workflow with measurable results, transparent AI limitations, and demonstrable access controls—not merely a polished interface or an AI chatbot.

---

## Decisions to confirm before implementation

1. The initial incident categories and the exact legal sources to support them.
2. Whether reports can be submitted anonymously or only through registered accounts.
3. Which case statuses reporters can see and which information remains internal.
4. Which documents may be uploaded, who can access them, and how long they are retained.
5. Whether the initial prototype will use synthetic data exclusively.
6. The institutional workflow and escalation rules to simulate.
7. The exact success criteria for the hackathon and the available development timeline.
>>>>>>> 7fa978dd9c2d00a401957e8334721a29a852db90
