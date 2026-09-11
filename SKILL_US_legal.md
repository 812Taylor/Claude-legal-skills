# SKILL.md — US Corporate Website Legal & Compliance Master Skill
# Scope: Commercial/company websites operated in or serving the United States
# Currency: 2026-09-11
# Important: This skill is a compliance engineering checklist, not legal advice.
# Never claim a site is "legally compliant" without identifying jurisdiction,
# business type, audience, data flows, and applicable state/federal rules.

## 0. Mission

When building, modifying, reviewing, or launching a company website for the United States:

1. Treat legal/compliance as part of the product, not as footer copy.
2. Determine which federal and state laws actually apply.
3. Inspect the implementation, not only the visible UI.
4. Map every data flow, third-party script, form, cookie, API, and storage location.
5. Do not invent legal facts, registrations, licenses, addresses, policies, or certifications.
6. Separate:
   - legally required items,
   - strongly recommended controls,
   - business-policy choices,
   - items that depend on state/industry facts.
7. When the facts are unknown, mark the item `REQUIRES CLIENT INPUT` rather than guessing.
8. Never use "we are fully compliant" as a default conclusion.
9. Before launch, run the Launch Compliance Gate in this file.

## 1. Baseline Legal Model

The United States does NOT have one universal website law or one universal "legal pages" requirement for all company websites.

The correct question is:

> Which federal, state, local, industry, contractual, platform, and accessibility rules apply to this exact business and website?

At minimum consider:

### Federal
- Federal Trade Commission Act / FTC unfair or deceptive acts principles
- FTC Endorsement Guides and advertising rules where applicable
- CAN-SPAM Act for commercial email
- Telephone Consumer Protection Act (TCPA) and implementing rules for covered calls/texts
- Children's Online Privacy Protection Act (COPPA), where applicable
- Americans with Disabilities Act (ADA), including applicable website/accessibility obligations
- Copyright Act
- Lanham Act / federal trademark law
- E-SIGN Act
- DMCA where user-generated content, takedown notices, or service-provider safe-harbor issues arise
- Gramm-Leach-Bliley Act (GLBA), if a covered financial institution
- HIPAA and related rules, if a covered entity/business associate
- Fair Credit Reporting Act (FCRA), where applicable
- State-specific unfair/deceptive acts laws
- Industry-specific federal statutes and regulations

### State / local
Always evaluate laws in:
- state of business formation,
- states where the business operates,
- states where consumers/users are targeted,
- states whose privacy or consumer laws apply to the business activity.

Potential topics include:
- comprehensive state privacy laws,
- health data laws,
- biometric/privacy laws,
- wiretap/communications laws,
- data-breach notification laws,
- children's privacy laws,
- automatic-renewal/subscription laws,
- telemarketing laws,
- text messaging rules,
- accessibility/consumer-protection rules,
- state-specific email requirements,
- tax and registration rules.

Do not assume that "the company is incorporated in Delaware" means only Delaware law matters.

## 2. Company Website Classification

Before coding or auditing, classify the website.

### Site type
- informational company website
- lead-generation website
- service-business website
- B2B website
- B2C website
- ecommerce
- SaaS
- marketplace
- membership/account portal
- booking/reservation website
- recruiting/careers site
- healthcare site
- finance/fintech site
- education site
- media/content site
- community/forum/user-generated-content site

### Audience
- B2B only
- consumers
- mixed B2B/B2C
- children/minors
- students
- patients
- job applicants
- regulated professionals

### Geography
Capture:
- company headquarters
- states where services are provided
- states intentionally targeted
- whether the site blocks certain jurisdictions
- whether the company has customers nationwide

### Data classification
Inventory:
- identifiers
- contact information
- account credentials
- commercial information
- geolocation
- internet activity
- device identifiers
- inferred profiles
- precise geolocation
- biometric data
- health information
- financial information
- employment data
- sensitive personal data
- children's data

Do not collect sensitive data merely because a field is convenient.

## 3. Required Legal Discovery Before Implementation

Ask for or determine:

### Business identity
- legal entity name
- DBA/trade name
- business address
- customer support contact
- privacy contact
- legal contact if different
- state(s) of formation
- EIN only when legally/business-use appropriate; never expose private tax records
- licenses/permits where relevant
- industry regulators
- professional licenses where applicable

### Commercial model
- free or paid
- one-time purchase
- subscription
- recurring billing
- free trial
- cancellation rules
- refunds
- digital goods
- physical goods
- services
- appointments
- deposits
- quotes
- contracts signed online

### Data/marketing
- analytics
- advertising
- retargeting
- email
- SMS
- CRM
- lead forms
- chat
- customer support
- account login
- user-generated content

### Vendors
For every vendor:
- vendor name
- service
- data received
- purpose
- region
- subprocessors
- contract / DPA status
- privacy commitments
- retention
- deletion process

## 4. Legal Pages / Public Notices

The exact set depends on the site. Common documents:

### Usually applicable
- Privacy Policy
- Terms of Use / Terms and Conditions where useful
- Contact information
- Cookie/Tracking preferences where applicable
- accessibility information / contact path where appropriate

### Often required or strongly relevant depending on business
- California privacy notice / CCPA-specific disclosures
- state privacy disclosures
- Notice at Collection
- "Do Not Sell or Share My Personal Information" pathway where required
- sensitive personal information controls where required
- SMS Terms
- SMS Consent language
- SMS opt-out instructions
- Email marketing disclosures
- subscription terms
- automatic-renewal terms
- refund/cancellation policy
- shipping policy
- returns policy
- warranty information
- acceptable use policy
- community guidelines
- DMCA policy/designated-agent information when relevant
- accessibility statement/contact method
- cookie notice
- biometric/health-data notices where required

Do not add pages merely for appearance. Each page must match the actual service.

## 5. Privacy — Core Federal/State Principle

There is no single comprehensive federal consumer privacy law covering every US company website.

Use a jurisdiction-by-jurisdiction matrix.

### Required privacy analysis
For each relevant state:
1. Does the law apply based on business size/revenue/volume/data thresholds?
2. Does it cover this data?
3. Is the business a controller/business or equivalent?
4. Is a processor/service-provider concept relevant?
5. What consumer rights apply?
6. Is there a Notice at Collection?
7. Is opt-out required for sale/sharing/targeted advertising?
8. Is consent required for sensitive data?
9. Are contracts with processors required?
10. Are assessments required?
11. Are universal opt-out mechanisms required?
12. Are appeal processes required?
13. Are response deadlines different?
14. Are dark-pattern restrictions applicable?

### Common state privacy-law themes
Depending on jurisdiction, consumers may have rights such as:
- access
- correction
- deletion
- data portability
- opt out of sale
- opt out of targeted advertising
- opt out of profiling
- limit/consent controls for sensitive information
- appeal a privacy-rights decision
- non-discrimination for exercising privacy rights

Never state that every state gives every right.

## 6. California — CCPA/CPRA Layer

If California privacy law applies, specifically investigate:
- notice at collection
- categories of personal information
- purposes
- retention or retention criteria where required
- categories of sources
- categories of recipients
- sale/sharing concepts
- targeted advertising concepts
- sensitive personal information
- consumer rights
- request verification
- correction/deletion workflows
- opt-out mechanisms
- Global Privacy Control / universal opt-out obligations where applicable
- required links/buttons
- service-provider/contractor requirements
- contractual data-use restrictions
- minors' consent requirements where applicable

Do not use a generic "CCPA compliant" footer as a substitute for implementation.

## 7. Privacy Requests

Create a real workflow for:
- access requests
- deletion requests
- correction requests
- portability requests
- opt-out requests
- targeted-advertising opt-out
- profiling opt-out
- appeal requests where applicable

Security requirements:
- do not disclose data to an unverified requester
- verify identity proportionately
- avoid collecting unnecessary identity data
- document request date
- document verification method
- document response
- document extensions/denials where permitted
- preserve an audit trail
- securely delete temporary verification material when no longer needed

## 8. Privacy Notice Content

A privacy policy should accurately describe:
- who operates the site
- what data is collected
- sources
- purposes
- legal/business basis when relevant
- categories of sharing/disclosure
- service providers
- advertising partners
- retention
- rights
- request process
- children's data handling
- international transfers where relevant
- security practices at an appropriate level of specificity
- changes to the policy
- contact methods
- effective/update date

Never include claims such as:
- "we never share data"
- "we do not track you"
- "your data is completely secure"
unless technically and legally substantiated.

## 9. Cookies & Tracking

Do NOT copy the European GDPR cookie model blindly into a US website.

Determine:
- which technologies are necessary
- which are analytics
- which are advertising
- which are personalization
- which are session/authentication
- which create or read identifiers
- whether the technology triggers state consent/opt-out rules
- whether wiretap/eavesdropping laws could be implicated
- whether a vendor receives page-level or form-input data
- whether the vendor builds profiles

### Inventory
Scan for:
- `_ga`
- Meta Pixel
- Google Ads
- TikTok Pixel
- LinkedIn Insight Tag
- Hotjar
- FullStory
- Clarity
- session replay
- chat widgets
- heatmaps
- affiliate tracking
- A/B testing
- fingerprinting
- ad-tech SDKs
- embedded video/maps
- fonts/CDNs

Do not rely only on browser cookies. Also inspect:
- localStorage
- sessionStorage
- IndexedDB
- request headers
- pixels
- POST bodies
- session replay
- server-side events.

## 10. Consent Architecture

Build consent/choice based on the legal requirements applicable to the site.

Where consent is required:
- obtain it before the relevant processing
- make the purpose understandable
- avoid deceptive UI
- do not preselect optional choices when not permitted
- provide a reasonable refusal path
- record the event
- honor the decision
- support withdrawal/revocation
- propagate preference to vendors
- stop or suppress processing when required

Where an opt-out mechanism is the legal model, do not falsely describe it as "consent."

## 11. Consumer Privacy Preference Signals

Where a jurisdiction requires recognition of a universal opt-out or browser signal:
- detect it correctly
- document how the signal is honored
- map it to the applicable opt-out(s)
- do not ignore it
- ensure downstream ad-tech respects the result
- test logged-out and logged-in flows where required
- test regional behavior.

The Global Privacy Control is especially important in California and other jurisdictions where laws/regulations require or recognize such signals.

## 12. Form Privacy

For every form define:
- fields
- purpose
- necessity
- destination
- retention
- access
- vendor
- privacy notice
- security controls

### Do not collect unnecessarily
Avoid fields such as:
- date of birth when age is irrelevant
- Social Security Number for generic contact requests
- driver's license number
- full payment card number
- precise home address when email is enough

### Forms must have
- accessible labels
- clear instructions
- understandable error messages
- consent/notice language when applicable
- anti-abuse protection that is privacy-conscious
- HTTPS
- server-side validation
- rate limiting
- CSRF protection where applicable.

## 13. Marketing Email — CAN-SPAM

For commercial email, inspect:
- truthful sender identity
- truthful subject line
- physical postal address
- clear advertising identification where required by law
- unsubscribe mechanism
- prompt processing of opt-outs
- no deceptive routing/header information
- vendor compliance
- suppression list handling

Do not make unsubscribe links require unnecessary login.

Do not send to a person again after a valid opt-out merely because a CRM export was refreshed.

Document suppression status.

## 14. SMS / Text Marketing — TCPA

Do not implement SMS marketing as if email rules were enough.

Determine:
- purpose of each message
- marketing vs transactional
- required consent
- wording of consent
- whether automated technology is used
- sender identity
- frequency
- disclosures
- terms
- privacy link
- HELP instructions
- STOP instructions
- opt-out handling
- revocation
- time-of-day rules
- applicable federal and state rules.

Never bundle SMS marketing consent into a deceptive unrelated checkbox.

Do not assume website terms alone establish valid messaging consent.

## 15. Children — COPPA

If the service is directed to children under 13, or you have actual knowledge you are collecting covered personal information from children:
- perform a COPPA analysis
- determine whether parental consent is required
- minimize data
- provide required notices
- implement parental-rights procedures
- control third-party disclosures
- retention/deletion
- age-screening only if legally appropriate and carefully designed.

Do not ask a child for unnecessary personal data.

If the product intentionally targets minors older than 13, check additional state children's/privacy laws as well.

## 16. Advertising / FTC

All claims must be truthful, substantiated where required, and not misleading.

Audit:
- "best"
- "number one"
- "guaranteed"
- "risk free"
- "free"
- "save X%"
- health/safety claims
- performance claims
- testimonials
- endorsements
- before/after images
- availability claims
- scarcity claims
- countdown timers
- pricing claims.

For every material marketing claim ask:

> What evidence supports this statement, and is the evidence current?

Do not create fake urgency:
- fake countdowns
- fake inventory
- fake user counts
- fake reviews
- fake awards
- fake testimonials.

## 17. Testimonials / Influencers / Reviews

If testimonials, endorsements, affiliates, or influencers are used:
- disclose material connections
- don't fabricate reviews
- don't manipulate review presentation deceptively
- don't selectively hide negative reviews in a misleading manner
- verify claims
- retain campaign records where appropriate
- ensure influencer instructions do not encourage illegal/deceptive claims.

Do not write a testimonial for a fictional person.

## 18. Pricing / Promotions

Display pricing accurately.

Audit:
- currency
- mandatory fees
- recurring charges
- setup fees
- shipping
- taxes as appropriate
- discount conditions
- trial conversion
- minimum term
- renewal price
- cancellation conditions
- eligibility restrictions.

Do not advertise "$0" and then reveal mandatory unavoidable charges only at the last step if the applicable law requires earlier disclosure.

Do not show a fake "was $999, now $499" comparison.

## 19. Subscriptions / Automatic Renewal

If the company sells recurring services:
- disclose recurring nature before purchase
- disclose price and renewal timing
- explain trial conversion
- explain cancellation
- comply with applicable state automatic-renewal laws
- capture required consent/affirmative action
- provide required confirmations
- provide easy cancellation method
- retain consent and renewal records.

Do not build a cancellation flow designed to trap users.

## 20. Ecommerce Contracting

For ecommerce, establish:
- product/service description
- total price
- mandatory fees
- availability
- delivery
- payment
- taxes
- refunds/returns
- cancellation
- warranty
- terms
- order confirmation
- customer support
- record retention.

Make the final action unambiguously indicate purchase/payment where applicable.

Do not hide material terms behind tiny text or misleading UI.

## 21. E-SIGN / Electronic Contracts

Where signatures/agreements are executed electronically:
- determine whether electronic records/signatures are appropriate
- provide required disclosures/consent
- ensure records are retainable and accessible
- avoid deceptive clickwrap
- preserve versioned terms
- preserve timestamps
- preserve evidence of assent.

For important agreements:
- use explicit clickwrap rather than passive browsewrap when appropriate
- place the agreement link immediately near the action
- record exact version accepted
- record time and relevant account/session data.

## 22. Terms of Use

If using Terms of Use, ensure they accurately describe:
- acceptable use
- intellectual property
- user content
- prohibited conduct
- disclaimers
- limitation of liability where enforceable
- dispute provisions where appropriate
- governing law where legally sensible
- termination
- account rules
- changes
- contact.

Never paste terms from another company.

Never include unenforceable or illegal terms as if they are certain to work.

## 23. Copyright

Every website asset needs a rights basis.

Audit:
- photos
- illustrations
- videos
- music
- fonts
- icons
- logos
- code
- templates
- stock assets
- AI-generated assets
- user submissions.

For each asset identify:
- creator/source
- license
- allowed use
- attribution requirement
- commercial-use permission
- modification rights
- expiration
- proof of license.

The U.S. Copyright Office confirms copyright can protect original writings, photographs, artwork, software, and other authorship appearing on websites.

Never assume:
- "it's on Google"
- "it's online"
- "I only used a small part"
- "AI made it"
means you have unrestricted commercial rights.

## 24. Trademarks

Audit:
- company name
- domain
- logos
- product names
- slogans
- competitor references
- customer logos.

Do not imply affiliation/endorsement without permission.

Before launch:
- search for conflicts
- verify ownership/license
- use branding consistently
- preserve trademark notices where appropriate.

## 25. User-Generated Content / DMCA

If the site allows users to post content:
- define content rules
- define license/grant language carefully
- provide reporting process
- investigate DMCA safe-harbor eligibility where relevant
- designate an agent if pursuing safe-harbor protections requires it
- publish required information
- create repeat-infringer policy as appropriate
- preserve notices and actions
- avoid automatic removal claims the business cannot support.

Do not say "DMCA protected" unless the actual conditions and policies are implemented.

## 26. Accessibility — ADA

Public-facing businesses can have ADA obligations. The DOJ states that Title III applies to businesses open to the public and that inaccessible web features can limit equal access to goods/services. The DOJ also points to WCAG as useful technical guidance.

Therefore build toward:
- semantic HTML
- keyboard access
- visible focus
- logical heading structure
- alt text
- sufficient text contrast
- accessible forms
- descriptive links/buttons
- captions/transcripts for media where needed
- no keyboard traps
- zoom/reflow support
- accessible error handling
- accessible navigation
- accessible modals/dialogs
- accessible authentication.

Do NOT claim that every private business website is subject to one identical WCAG statutory standard. Applicability and technical expectations depend on the business, legal theory, jurisdiction, and current rules.

### Accessibility testing
Use:
- automated scan
- keyboard-only test
- screen-reader spot checks
- zoom test
- reduced-motion test
- focus-order test
- form error test
- contrast test
- mobile accessibility test.

Automated scores are not proof of legal compliance.

## 27. Accessibility Statement

When appropriate, include:
- accessibility commitment
- contact method for accessibility problems
- expected response/support path
- known limitations only if accurate
- compatible contact alternative.

Do not publish fake claims such as "100% accessible" without evidence.

## 28. California and Other State Consumer Laws

Run a state matrix for:
- privacy
- data breach
- automatic renewal
- telemarketing
- text messaging
- subscriptions
- consumer cancellation
- accessibility
- health data
- biometrics
- children's data
- deceptive pricing
- sweepstakes
- gift cards
- shipping/returns
- professional licensing.

Do not assume the privacy policy covers all consumer laws.

## 29. Data Breach Readiness

Build a breach-response process.

Maintain:
- data inventory
- vendor list
- incident contacts
- logging
- backup plan
- containment plan
- evidence preservation
- legal escalation path
- state-by-state breach notification matrix.

Do not promise a fixed notification time without checking the applicable law.

## 30. Security Engineering

For company websites implement, as appropriate:
- HTTPS
- HSTS
- secure cookies
- HttpOnly
- SameSite
- CSP where practical
- input validation
- output encoding
- CSRF defense where applicable
- authentication controls
- MFA for privileged/admin access
- secure password hashing
- session expiration
- rate limiting
- bot protection
- least privilege
- secret management
- dependency updates
- vulnerability scanning
- backups
- restore testing
- logging/monitoring
- intrusion detection where appropriate.

Never store plaintext passwords.

Never commit secrets/API keys to source control.

Never expose private customer data in client-side JavaScript.

## 31. Payments

Prefer a reputable hosted/tokenized payment processor rather than handling raw card data.

Determine:
- PCI DSS scope
- cardholder-data flow
- payment-provider contract
- refund process
- chargeback process
- billing descriptors
- recurring-payment rules.

Never collect raw card details in a generic form unless the security/compliance architecture explicitly supports it.

## 32. Healthcare

If healthcare is involved, perform separate HIPAA analysis.

Determine:
- covered entity status
- business associate status
- PHI
- patient portal
- forms
- analytics/session-replay impact
- vendor BAAs
- minimum necessary considerations
- privacy/security rules
- state health-data laws.

Never send sensitive health information to an advertising/analytics platform merely because it is easy to install.

## 33. Financial Services

If the company provides financial products/services, check applicable:
- GLBA
- FTC Safeguards Rule where applicable
- financial privacy rules
- securities laws
- state financial regulations
- money-transmission rules
- lending rules
- advertising requirements.

This is not a normal corporate-site compliance project.

## 34. Employment / Careers

For recruiting pages:
- protect applicant data
- state the purpose of collection
- avoid unnecessary sensitive data
- provide accessible application forms
- secure resumes
- control retention
- review applicant tracking vendors
- consider state/local employment/privacy rules.

Do not ask applicants for SSNs before necessary.

## 35. Location / Maps

For map services, inspect:
- API key exposure
- vendor terms
- data transfer
- tracking
- location permissions
- attribution requirements
- privacy implications.

Use least-privileged API keys and domain restrictions where supported.

## 36. Third-Party Scripts

Every `<script>` is a compliance and supply-chain review item.

For each script record:
- vendor
- purpose
- data accessed
- request destinations
- cookies/storage
- whether it executes before user choice
- whether it reads form input
- whether it captures keystrokes/session replay
- retention
- geographic transfer
- legal basis/opt-out basis where applicable.

Do not install scripts that were not approved in the vendor/data inventory.

## 37. External Fonts / Assets

Prefer self-hosting where practical when it reduces unnecessary third-party requests.

For third-party fonts/CDNs verify:
- license
- vendor
- requests
- IP/data transfer
- privacy statement.

## 38. Analytics

For each analytics system:
- identify vendor
- identify event schema
- avoid transmitting unnecessary personal data
- avoid sending form values, passwords, health data, payment data
- configure retention
- configure IP/location settings if available
- honor privacy choices
- document use.

Do not put names/emails into analytics event parameters unless there is a documented lawful reason and architecture.

## 39. AI Features

If using AI/chatbots:
- disclose AI interaction where appropriate
- define what user data reaches the model/provider
- do not send unnecessary confidential data
- check vendor retention/training terms
- create abuse controls
- secure prompts/system instructions
- prevent prompt injection from exposing secrets
- prevent cross-user data leakage
- do not fabricate legal/medical/financial certainty
- add human escalation for high-risk use cases.

## 40. SEO Compliance

SEO is not only a ranking concern.

Audit:
- truthful titles
- truthful descriptions
- no hidden deceptive text
- no fake reviews
- no misleading structured data
- no doorway pages intended to deceive
- correct business identity
- accurate contact details
- correct `robots.txt`
- correct canonical tags
- no accidental indexing of private pages
- `noindex` for sensitive/admin areas.

Do not put personal/private data in URLs.

## 41. Search / Account / Private Content

Protect:
- account pages
- invoices
- applications
- internal documents
- support tickets
- private uploads.

Implement authorization on the server.

Never rely only on hiding a page link.

Never assume an unguessable URL is authorization.

## 42. Error Pages / Logs

Error messages shown to users must not reveal:
- stack traces
- database names
- internal paths
- API keys
- tokens
- vendor secrets
- customer data.

Logs should be reviewed for accidental personal/sensitive data.

## 43. Data Retention / Deletion

Every meaningful data category should have:
- purpose
- owner
- retention rule
- deletion/anonymization method
- legal hold exception process
- backup treatment.

Do not keep lead submissions forever just because storage is cheap.

## 44. Vendor Contracts

For privacy/security-sensitive vendors, review:
- DPA/privacy addendum
- processor/service-provider terms
- subprocessor list
- security commitments
- breach notification
- deletion/return
- audit rights where relevant
- international transfers
- data-use restrictions
- whether vendor can use data for its own advertising/AI training.

Do not label a vendor "service provider" merely because its marketing page says so.

## 45. International Visitors

A US company may still have obligations regarding users outside the United States.

Before declaring a website "US only", determine whether:
- the site is accessible globally
- products are sold internationally
- EU/EEA users are targeted
- UK users are targeted
- other privacy regimes may apply.

If the business intentionally targets Europe, perform a separate GDPR/UK analysis.

## 46. Taxes

A corporate website does not itself determine tax obligations.

For ecommerce/services:
- identify nexus
- determine sales tax obligations by state
- configure tax collection correctly
- verify marketplace facilitator rules
- maintain invoices/records
- ensure displayed prices are not misleading.

Do not promise "all taxes included" unless the business has verified the claim.

## 47. Domain / DNS / Email Security

Implement:
- SPF
- DKIM
- DMARC
- appropriate DMARC monitoring/enforcement strategy
- domain registrar MFA
- DNS protection
- auto-renewal
- registrar lock where available.

Protect business email because website forms often feed into email systems.

## 48. Accessibility-Safe UI Components

Every component must pass:
- keyboard navigation
- focus management
- semantic role
- accessible name
- accessible state
- screen-reader behavior
- reduced motion
- zoom
- touch target usability.

This includes:
- navbar
- dropdown
- mega menu
- modal
- accordion
- tabs
- carousel
- cookie/privacy panel
- contact form
- login
- checkout
- chatbot.

Avoid unnecessary ARIA. Native HTML is preferred where possible.

## 49. Dark Patterns — Prohibited Design Philosophy

Do not design:
- deceptive consent banners
- hidden close buttons
- preselected marketing choices where not appropriate
- confusing unsubscribe
- disguised ads
- fake system warnings
- fake countdowns
- fake stock
- hidden fees
- confirmshaming
- forced continuity
- cancellation mazes
- visual tricks to make "accept" easier while hiding "reject".

## 50. Required Code Review

Before launch inspect:
- all HTML files
- CSS
- JS/TS
- package dependencies
- environment variables
- backend endpoints
- third-party scripts
- API requests
- cookies
- localStorage/sessionStorage
- network requests
- forms
- hidden fields
- iframes
- redirects
- analytics payloads
- robots/noindex
- sitemap
- headers.

Do not limit legal review to visible text.

## 51. Automated Compliance Audit

Run:
- HTML validation
- accessibility scanner
- Lighthouse/accessibility checks
- dependency vulnerability scan
- secret scan
- link checker
- cookie/storage inspection
- network request audit
- security headers audit
- form submission test
- mobile test
- keyboard test.

Automated tools are evidence, not legal certification.

## 52. Human Legal Review Triggers

Escalate to qualified US counsel when:
- regulated industry
- children
- health data
- biometric data
- precise location
- large-scale profiling
- financial services
- nationwide ecommerce with many states
- subscriptions/auto-renewal
- telemarketing/SMS
- high-risk user-generated content
- custom liability/dispute clauses
- accessibility litigation risk
- privacy requests are denied
- breach occurs
- acquisition/merger or major data migration
- business makes strong health, financial, safety, or performance claims.

## 53. Launch Compliance Gate

Do NOT mark `READY` until all applicable boxes are confirmed.

### Identity
- [ ] Legal company identity confirmed
- [ ] Contact address confirmed
- [ ] Business contact confirmed
- [ ] Licenses checked
- [ ] Industry identified

### Privacy
- [ ] Data inventory complete
- [ ] Data flows mapped
- [ ] State privacy applicability reviewed
- [ ] Privacy policy matches implementation
- [ ] Request workflow works
- [ ] Vendor list complete
- [ ] Retention defined
- [ ] deletion process tested
- [ ] sensitive data handling reviewed
- [ ] universal opt-out requirements checked

### Tracking
- [ ] Cookie/storage inventory complete
- [ ] analytics inventory complete
- [ ] advertising inventory complete
- [ ] session replay reviewed
- [ ] consent/opt-out behavior tested
- [ ] vendor scripts respect preferences

### Marketing
- [ ] email rules reviewed
- [ ] unsubscribe tested
- [ ] SMS rules reviewed if applicable
- [ ] STOP/HELP behavior tested if applicable
- [ ] advertising claims substantiated
- [ ] endorsements/reviews reviewed

### Ecommerce
- [ ] pricing reviewed
- [ ] fees reviewed
- [ ] recurring terms reviewed
- [ ] trial conversion reviewed
- [ ] returns/refunds reviewed
- [ ] cancellation tested
- [ ] checkout terms reviewed
- [ ] confirmation emails tested

### Accessibility
- [ ] keyboard test
- [ ] screen-reader spot check
- [ ] headings
- [ ] alt text
- [ ] contrast
- [ ] forms
- [ ] focus
- [ ] dialogs
- [ ] mobile
- [ ] zoom/reflow
- [ ] captions/transcripts where applicable

### Security
- [ ] HTTPS
- [ ] security headers
- [ ] secrets scan
- [ ] dependency scan
- [ ] auth tested
- [ ] authorization tested
- [ ] rate limits
- [ ] input validation
- [ ] logs reviewed
- [ ] backups
- [ ] incident plan

### IP
- [ ] image licenses
- [ ] font licenses
- [ ] icon licenses
- [ ] code licenses
- [ ] music/video licenses
- [ ] trademark review
- [ ] user-content terms

### Technical
- [ ] no broken links
- [ ] no accidental staging pages
- [ ] no private pages indexed
- [ ] forms deliver correctly
- [ ] 404/500 pages safe
- [ ] analytics payloads clean
- [ ] robots.txt correct
- [ ] sitemap correct
- [ ] DNS/email security configured

## 54. Evidence Pack

For a serious company website, maintain an internal compliance evidence folder containing:

- website architecture
- data map
- vendor register
- privacy-policy version
- terms version
- cookie inventory
- consent configuration
- screenshots of key legal UI
- accessibility test reports
- security test reports
- license records
- trademark records
- marketing claim substantiation
- SMS/email consent records where relevant
- subscription/checkout screenshots
- legal-review notes
- release/version history
- incident response contacts
- retention schedule.

Do not store unnecessary sensitive personal data in the evidence pack.

## 55. Release Procedure

Every legal/compliance-sensitive release should follow:

1. Identify changed functionality.
2. Re-run applicable legal classification.
3. Check new data collection.
4. Check new vendors.
5. Check new scripts.
6. Check new marketing claims.
7. Check accessibility impact.
8. Check state-law impact.
9. Update legal documents where required.
10. Test production behavior.
11. Record release evidence.
12. Deploy.

A new analytics script is not "just frontend."

A new form field is not "just UI."

A new subscription option is not "just pricing."

A new chatbot is not "just UX."

## 56. Claude Coding Rules

When Claude is asked to build or modify a US company website:

### MUST
- inspect existing code before changing it
- preserve existing compliant behavior
- identify legal-risk changes
- avoid invented company facts
- avoid invented legal claims
- keep privacy text synchronized with actual implementation
- use semantic accessible HTML
- avoid unnecessary trackers
- use secure defaults
- flag jurisdiction-specific questions
- leave `REQUIRES CLIENT INPUT` markers where facts are missing
- document assumptions in comments or a compliance note
- test forms and navigation
- test third-party requests
- test keyboard accessibility

### MUST NOT
- claim "legally compliant" without a jurisdiction-specific review
- invent a legal address
- invent a privacy contact
- invent a registration number
- invent licenses/certifications
- invent customer testimonials
- add tracking without documenting it
- collect unnecessary sensitive data
- copy another company's legal text verbatim
- use fake urgency
- hide material fees
- create dark patterns
- hardcode secrets
- store passwords in plaintext
- expose private API keys
- upload customer data to unapproved AI services

## 57. Default Safe Technical Architecture

For a normal informational corporate site, prefer:

- static/SSR pages where practical
- minimal third-party JavaScript
- self-hosted assets where practical
- semantic HTML
- accessible forms
- HTTPS
- secure headers
- no unnecessary account system
- no unnecessary personal data
- privacy-conscious analytics
- no session replay by default
- no ad pixels by default
- explicit vendor inventory
- version-controlled legal pages
- simple contact workflow
- secure server-side email/form processing

## 58. Default Site Structure

For a normal corporate website:

/
 /about
 /services
 /contact
 /careers              (if applicable)
 /privacy
 /terms                (if applicable)
 /accessibility        (if appropriate)
 /cookie-preferences   (if applicable)
 /sms-terms            (if applicable)
 /refunds              (if applicable)
 /shipping             (if applicable)

Footer should make required/legal information easy to find without deceptive navigation.

## 59. Final Output Format for Claude

When completing a compliance-oriented website task, report:

### STATUS
`READY`, `READY WITH CONDITIONS`, or `BLOCKED`

### APPLICABLE JURISDICTIONS
List states/federal regimes actually assessed.

### LEGAL SURFACE
List:
- privacy
- marketing
- accessibility
- ecommerce
- IP
- industry
- security
- state-specific items

### IMPLEMENTED
List actual controls implemented.

### CLIENT INPUT REQUIRED
List every fact the developer could not safely invent.

### OPEN LEGAL QUESTIONS
List issues needing counsel.

### TESTS RUN
List technical/accessibility/privacy/security tests.

### REMAINING RISK
Use:
- Low
- Medium
- High
- Critical

Never turn "not tested" into "compliant."

## 60. Primary Sources to Prefer

For US legal research, prefer official sources:
- FTC: https://www.ftc.gov/
- ADA.gov / U.S. Department of Justice: https://www.ada.gov/
- U.S. Copyright Office: https://www.copyright.gov/
- Congress / U.S. Code: https://uscode.house.gov/
- Federal Register: https://www.federalregister.gov/
- CFPB: https://www.consumerfinance.gov/
- FCC: https://www.fcc.gov/
- HHS / HIPAA: https://www.hhs.gov/hipaa/
- IRS: https://www.irs.gov/
- USPTO: https://www.uspto.gov/
- State attorney general/privacy regulator websites
- official state legislative/code websites

Use secondary sources only as navigation/context, then verify the controlling rule in an official source when possible.

## 61. Important Current-Law Note

Current law changes. For any task involving:
- current privacy rules,
- current accessibility rules,
- recent FTC/FCC interpretations,
- state privacy thresholds,
- new subscription laws,
- current enforcement positions,
- current tax rules,
- current platform policies,

perform a fresh web verification before finalizing.

Do not rely on a static copy of this file as proof that a legal rule remains unchanged.

## 62. Core Principle

The objective is NOT:

> "Put Privacy Policy and Terms in the footer."

The objective is:

> "Make the actual product behavior, data flows, marketing, accessibility, contracts, security controls, and legal documents agree with each other and with the laws applicable to the business."

If implementation and policy disagree, treat the website as `NOT READY` until the discrepancy is resolved or counsel approves a documented approach.
