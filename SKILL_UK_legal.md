# SKILL.md — UK Company Website Compliance Engineer
# Legal / technical baseline: 11 September 2026
# Jurisdiction: United Kingdom
# Intended user: Claude Code / Claude Desktop / AI coding agent
#
# IMPORTANT:
# This skill is a compliance-oriented engineering specification, not legal advice.
# UK requirements vary by business model, UK nation, sector, customer location,
# company structure, technology stack and data flows.
# Never state that a website is "legally compliant" merely because this checklist passes.
# Instead report: PASS / FAIL / NEEDS LEGAL REVIEW / NOT APPLICABLE.
#
# CURRENT-LAW RULE:
# The baseline date for this file is 11 September 2026.
# The Data (Use and Access) Act 2025 (DUAA) data-protection changes are treated as
# in force. The ICO confirmed on 19 June 2026 that all data-protection provisions
# of DUAA were in force. The ICO's final Storage and Access Technologies guidance
# was published 29 April 2026. Always verify later changes before launch.
#
# PRIMARY AUTHORITATIVE SOURCES TO VERIFY:
# - https://ico.org.uk/  (ICO)
# - https://www.gov.uk/  (UK Government guidance)
# - https://www.legislation.gov.uk/  (official legislation)
# - https://www.asa.org.uk/  (ASA / CAP)
# - https://www.fca.org.uk/  (financial services, when applicable)
# - https://www.ofcom.org.uk/  (communications / Online Safety, when applicable)
#
# Core legislation / regimes to consider:
# - UK GDPR, as amended by DUAA
# - Data Protection Act 2018, as amended by DUAA
# - Data (Use and Access) Act 2025
# - Privacy and Electronic Communications Regulations 2003 (PECR), as amended
# - Companies Act 2006 and company-information rules
# - Electronic Commerce Regulations 2002
# - Consumer Contracts Regulations 2013 (where applicable)
# - Consumer Rights Act 2015
# - Digital Markets, Competition and Consumers Act 2024 (especially consumer/subscription rules
#   as and when commenced)
# - Consumer Protection from Unfair Trading regime (including the current post-DMCC framework)
# - Equality Act 2010
# - Copyright, Designs and Patents Act 1988
# - Trade Marks Act 1994
# - Defamation Act 2013 (content-dependent)
# - Online Safety Act 2023 (platform/user-content scope only)
# - Investigatory / interception / communications rules where relevant
# - sector-specific legislation
#
# =========================
# 0. OPERATING PRINCIPLES
# =========================
#
# RULE 0.1 — DO NOT GUESS
# Never invent a legal requirement, statutory deadline, company identifier,
# regulator, fee, exemption, privacy right, accessibility obligation, or
# wording requirement. Verify against current official UK sources.
#
# RULE 0.2 — ASK ONLY WHEN MATERIAL
# If facts are missing, make a reasonable provisional assumption and mark it.
# Do not block normal development unnecessarily.
#
# RULE 0.3 — JURISDICTION FIRST
# Determine:
#   - England / Wales / Scotland / Northern Ireland
#   - where the company is incorporated
#   - where customers are located
#   - whether the site targets UK consumers
#   - whether the business is regulated
# Some rules differ between UK nations.
#
# RULE 0.4 — COMPANY WEBSITE ≠ ONLINE SHOP
# A brochure/company site can have fewer consumer-contract obligations than
# a site that accepts orders, subscriptions, deposits or bookings.
#
# RULE 0.5 — THIRD PARTIES ARE PART OF THE WEBSITE
# Scan every third-party script, font, SDK, image, iframe, API, analytics tool,
# CAPTCHA, chat widget, CDN and payment provider.
#
# RULE 0.6 — PRIVACY BY DESIGN
# Default to data minimisation, purpose limitation, least privilege,
# short retention, secure defaults and no non-essential tracking before a lawful basis
# / consent has been established where required.
#
# RULE 0.7 — NEVER HIDE COMPLIANCE
# Legal notices must be easy to find and should not be buried in menus that users
# cannot reasonably access.
#
# RULE 0.8 — DOCUMENT DECISIONS
# Produce a compliance manifest:
#   docs/compliance/uk-website-compliance.md
# containing every applicable module, assumption, evidence, owner and review date.
#
# =========================
# 1. PROJECT INTAKE
# =========================
#
# Before coding, classify the site.
#
# Required intake questions:
# - Company name
# - Legal entity type
# - Registered jurisdiction
# - Registered office / principal address
# - Company registration number (if applicable)
# - VAT registration status
# - Nature of business
# - Physical products / services / digital content
# - B2B / B2C / both
# - UK only / international
# - Countries targeted
# - Does the site sell online?
# - Does it take deposits or bookings?
# - Does it create recurring subscriptions?
# - Does it create customer accounts?
# - Does it collect leads?
# - Does it send marketing email/SMS/calls?
# - Does it process children's data?
# - Does it use profiling / automated decisions / AI?
# - Does it allow user-generated content?
# - Does it contain reviews/comments?
# - Does it use advertising / affiliate marketing?
# - Does it use analytics, ad pixels or session replay?
# - Does it use payment providers?
# - Does it embed third-party content?
# - Is the service accessibility-sensitive / subject to specific duties?
# - Is the company in a regulated sector?
#
# Set:
#   SITE_CLASS =
#     COMPANY_BROCHURE
#     LEAD_GENERATION
#     B2B_SERVICE
#     B2C_SERVICE
#     ECOMMERCE
#     SAAS
#     SUBSCRIPTION
#     BOOKING
#     MARKETPLACE
#     USER_GENERATED_CONTENT
#     PUBLISHER / EDITORIAL
#     REGULATED_SECTOR
#
# =========================
# 2. ALWAYS-ON UK COMPANY SITE MODULE
# =========================
#
# 2.1 COMPANY IDENTITY
# If the site belongs to a UK company, verify the required company details for
# the applicable company type and medium.
#
# At minimum, investigate whether the website should disclose:
# - registered company name
# - company number
# - registered office address
# - place of registration
# - legal form where relevant
# - appropriate contact details
# - VAT number where relevant
# - trading name vs legal entity distinction
#
# Do not fabricate any of these.
#
# 2.2 WEBSITE FOOTER
# Recommended standard structure:
#   About
#   Contact
#   Privacy
#   Cookies / Cookie settings (where applicable)
#   Terms
#   Accessibility / accessibility information where relevant
#   Company details
#
# 2.3 COMPANY NAME / URL / CLAIMS
# Review company name, domain name and on-page claims for misleading impressions.
# ASA/CAP guidance confirms that company names and URLs can contribute to the
# overall impression of an advertisement.
#
# =========================
# 3. PRIVACY — UK GDPR + DPA 2018 + DUAA
# =========================
#
# Treat these as the core UK privacy stack.
#
# 3.1 ACCOUNTABILITY
# The implementation must support:
# - records of processing where required
# - lawful basis analysis
# - data minimisation
# - retention periods
# - rights handling
# - processor management
# - security measures
# - breach management
# - international-transfer assessment
#
# 3.2 PRIVACY NOTICE
# Create a privacy notice that matches actual processing.
# Never generate generic language that contradicts the code.
#
# Include, where applicable:
# - identity and contact details of controller
# - DPO details if one is required/appointed
# - categories of personal data
# - purposes
# - lawful bases
# - legitimate-interest explanation where relied upon
# - recipients / categories of recipients
# - international transfers
# - safeguards for transfers
# - retention / criteria
# - individual rights
# - complaint route to ICO
# - source of data if not collected directly
# - automated decision-making / profiling information where applicable
#
# 3.3 LAWFUL BASIS ENGINE
# For every processing activity classify:
#   CONSENT
#   CONTRACT
#   LEGAL_OBLIGATION
#   VITAL_INTERESTS
#   PUBLIC_TASK
#   LEGITIMATE_INTERESTS
#
# Never use consent merely because it is convenient.
# Never use legitimate interests where the processing requires consent under PECR.
#
# 3.4 CONSENT
# Consent must be:
# - specific
# - informed
# - freely given
# - unambiguous
# - recorded
# - withdrawable
#
# Record:
# - timestamp
# - version of notice
# - purpose
# - source / context
# - scope
# - evidence of action
#
# 3.5 DATA SUBJECT RIGHTS
# Build operational support for, where applicable:
# - access
# - rectification
# - erasure
# - restriction
# - portability
# - objection
# - consent withdrawal
# - rights concerning solely automated decisions / profiling
#
# Do not hard-code old pre-DUAA assumptions. Verify current exemptions,
# procedures and statutory details against current ICO guidance.
#
# 3.6 CHILDREN
# Where children may use the service, implement age-aware and risk-based
# privacy design. Verify current DUAA / UK GDPR / ICO children's-data guidance.
#
# 3.7 AUTOMATED DECISION-MAKING / AI
# If decisions are made by algorithms:
# - identify whether Article 22-type rules apply
# - assess safeguards and human involvement
# - document logic and significance where disclosure is required
# - ensure the privacy notice is accurate
# - do not claim "human review" unless genuine and effective
#
# =========================
# 4. ICO REGISTRATION / DATA PROTECTION FEE
# =========================
#
# Determine whether the organisation is required to pay the ICO data protection fee.
# Use the ICO's current fee self-assessment / registration information.
# Do not assume "small company = exempt".
#
# Include a task in the compliance manifest:
#   "ICO fee / registration status verified on <date>"
#
# =========================
# 5. COOKIES / PECR / STORAGE & ACCESS TECHNOLOGIES
# =========================
#
# This module is mandatory whenever the site uses:
# - cookies
# - localStorage / sessionStorage
# - pixels
# - device fingerprinting
# - scripts/tags
# - link decoration / navigational tracking
# - similar storage/access technologies
#
# The ICO's final Storage and Access Technologies guidance is dated 29 April 2026.
#
# 5.1 INVENTORY
# Generate a machine-readable inventory:
#   cookie / key
#   technology
#   provider
#   purpose
#   type
#   duration
#   first/third party
#   domain
#   data collected
#   where data is sent
#   whether PECR exception applies
#   consent category
#
# 5.2 NECESSARY VS NON-ESSENTIAL
# Evaluate whether the technology falls within a valid PECR exception.
# Do not label something "strictly necessary" solely because marketing wants it.
#
# 5.3 CONSENT UI
# Where consent is required:
# - make the choice meaningful
# - explain purposes clearly
# - provide a simple means of objecting / refusing where required
# - allow withdrawal
# - do not secretly activate rejected categories
# - log consent
#
# 5.4 LOAD ORDER
# Non-essential trackers must not fire before the required permission is in place.
#
# 5.5 MULTI-PURPOSE TECHNOLOGY
# If one technology serves several purposes, assess each purpose.
# Do not assume a single "analytics" label covers advertising, profiling, fraud,
# personalisation and measurement.
#
# 5.6 TESTING
# Use:
# - fresh browser profile
# - consent accept
# - consent reject
# - partial choices
# - withdrawal
# Verify requests in browser network tools.
#
# =========================
# 6. DIRECT MARKETING — PECR
# =========================
#
# If the site collects marketing contacts, explicitly model:
# - email marketing
# - SMS marketing
# - automated calls
# - live marketing calls
# - other electronic marketing
#
# For consent-based marketing:
# - specific positive action
# - clear wording
# - named organisation / appropriate scope
# - records
# - easy withdrawal / unsubscribe
#
# For "soft opt-in":
# - verify each statutory condition before using it
# - do not use the exception as a blanket permission
#
# PECR has been amended by DUAA. Verify current ICO guidance as of launch.
#
# EMAIL / SMS UI:
# Never pre-tick marketing consent by default.
# Separate service communications from promotional marketing.
#
# =========================
# 7. CONTACT FORMS / LEAD FORMS
# =========================
#
# For every form:
# - document each field
# - identify lawful basis
# - minimise data
# - avoid collecting sensitive data unless necessary
# - show the relevant privacy explanation
# - protect against spam
# - use HTTPS
# - validate server-side
# - prevent injection
# - rate-limit
# - avoid exposing email addresses unnecessarily
#
# If a form contains a marketing checkbox:
# - it must not be bundled into "required" unless genuinely necessary
# - record the choice separately
# - state what marketing will be sent
#
# =========================
# 8. SECURITY
# =========================
#
# Security controls should be proportionate to risk and data sensitivity.
#
# REQUIRED REVIEW:
# - HTTPS everywhere
# - HSTS where appropriate
# - secure cookies
# - HttpOnly for session cookies where appropriate
# - SameSite configured intentionally
# - CSRF protection where relevant
# - XSS prevention
# - SQL/NoSQL injection prevention
# - output encoding
# - input validation
# - authorization checks
# - least privilege
# - secret management
# - no API keys in frontend source unless intentionally public
# - dependency patching
# - security headers
# - CSP where practical
# - clickjacking protections
# - MIME sniffing protections
# - rate limiting
# - bot abuse controls
# - backups
# - restore testing
# - logging and monitoring
# - admin interface protection
#
# Never claim compliance because "we use HTTPS".
#
# =========================
# 9. DATA BREACH / INCIDENT RESPONSE
# =========================
#
# Provide a runbook:
# 1. detect
# 2. contain
# 3. preserve evidence
# 4. assess data affected
# 5. assess risk to individuals
# 6. determine regulatory reporting obligations
# 7. determine individual notification obligations
# 8. document decisions
# 9. remediate
#
# Verify the current UK GDPR / DPA / DUAA rules and ICO guidance for notification
# timing and exceptions at the time of the incident.
#
# =========================
# 10. PROCESSORS / VENDORS
# =========================
#
# For every external vendor determine:
# - controller vs processor role
# - processing purposes
# - data categories
# - contract requirements
# - sub-processors
# - security
# - retention
# - deletion / return
# - international transfers
# - incident terms
#
# Where Article 28-style processor requirements apply, use a suitable contract.
#
# =========================
# 11. INTERNATIONAL DATA TRANSFERS
# =========================
#
# Detect if personal data can leave the UK.
# Common examples:
# - US cloud
# - US analytics
# - CRM
# - email marketing platform
# - support chat
# - CDN
# - error monitoring
# - payment services
#
# Verify:
# - adequacy
# - UK transfer mechanism
# - applicable contractual safeguards
# - transfer risk assessment / required assessment
# - supplementary measures
# - onward transfers
#
# Do not assume "vendor is GDPR compliant" = UK transfer compliance.
#
# =========================
# 12. THIRD-PARTY SERVICES
# =========================
#
# Build a THIRD_PARTY_REGISTER with:
# - provider
# - service
# - domain
# - purpose
# - cookies/storage
# - personal data
# - country
# - lawful basis
# - consent dependency
# - contract
# - transfer basis
# - privacy-policy URL
# - owner
#
# Explicitly review:
# - Google Fonts
# - Google Maps
# - YouTube
# - Vimeo
# - reCAPTCHA
# - hCaptcha
# - Cloudflare
# - Meta Pixel
# - TikTok
# - LinkedIn Insight
# - Hotjar / session replay
# - Sentry
# - Intercom / chat
# - Calendly / booking
# - HubSpot / CRM
# - analytics
# - payment providers
#
# Do not assume any vendor is "safe" merely because it is popular.
#
# =========================
# 13. ACCESSIBILITY
# =========================
#
# Do not automatically apply public-sector accessibility law to a private company.
# First determine whether the service is within a specific statutory regime.
#
# Independently, design websites to strong accessibility standards:
# - semantic HTML
# - keyboard navigation
# - visible focus
# - sensible heading structure
# - accessible names
# - labels
# - error identification
# - sufficient contrast
# - resize / zoom resilience
# - captions/transcripts where relevant
# - reduced-motion consideration
# - no color-only meaning
# - touch target usability
# - screen-reader compatibility
#
# Use WCAG 2.2 AA as an engineering benchmark unless a different legal/contractual
# standard applies.
#
# For UK private-sector businesses, also investigate Equality Act 2010 duties,
# including reasonable adjustments where relevant to the service.
#
# =========================
# 14. E-COMMERCE / ONLINE SALES
# =========================
#
# Activate for any online order, booking, paid service, digital content or subscription.
#
# Before order, review whether the customer is given:
# - trader identity
# - contact details
# - address
# - product/service description
# - main characteristics
# - total price including taxes where required
# - additional charges
# - delivery options/costs
# - payment methods
# - minimum term
# - renewal / termination conditions
# - cancellation rights and exceptions
# - complaints information where applicable
# - terms the consumer can save/reproduce
#
# GOV.UK online-selling guidance specifically highlights making payment obligation clear,
# delivery options/costs, promotions, order steps, error correction, available languages,
# savable T&Cs, email, VAT number where registered and other pre-contract information.
#
# =========================
# 15. CHECKOUT UX
# =========================
#
# The checkout must make it unambiguous that the customer is committing to payment.
# Use clear wording such as "Pay now" where appropriate.
#
# Before submission:
# - show basket summary
# - show price
# - show recurring nature where applicable
# - show key charges
# - show required terms / confirmations
# - give a practical way to correct errors
#
# Never use dark patterns to obscure the payment obligation.
#
# =========================
# 16. CONSUMER CANCELLATION / 14-DAY RIGHTS
# =========================
#
# For in-scope distance contracts, implement and verify:
# - cancellation information
# - cancellation process
# - standard cancellation form where required
# - refund workflow
# - return process
# - exceptions
#
# GOV.UK states that online customers generally have a 14-day cancellation right,
# subject to exceptions and contract type.
#
# For digital downloads/streaming:
# - identify the consent and acknowledgement requirements for loss of cancellation rights
# - obtain the required express agreement before instant supply
# - reflect it in the confirmation.
#
# Do not write "no refunds" as a blanket rule for consumer contracts if statutory rights apply.
#
# =========================
# 17. CONSUMER RIGHTS ACT 2015
# =========================
#
# For consumer goods/services/digital content, review:
# - satisfactory quality
# - fitness for purpose
# - conformity with description
# - reasonable care and skill for services
# - digital-content consumer rights
# - remedies
#
# Marketing promises can become part of the customer's expectations.
#
# =========================
# 18. SUBSCRIPTIONS / AUTO-RENEWAL
# =========================
#
# Activate for:
# - monthly/annual SaaS
# - memberships
# - recurring product boxes
# - streaming
# - paid newsletters
# - recurring service plans
#
# Use a dedicated subscription compliance module.
#
# Review the current Digital Markets, Competition and Consumers Act 2024
# and its commencement status before launch.
#
# Model:
# - initial price
# - recurring price
# - billing interval
# - trial
# - trial-to-paid transition
# - renewal
# - reminder requirements where in force
# - cancellation
# - renewal cooling-off rights where applicable
# - refund logic
# - price increases
# - consumer communications
#
# Never silently turn a free trial into a paid recurring subscription.
#
# =========================
# 19. CANCELLATION / TERMINATION UI
# =========================
#
# Where a legal cancellation route is required:
# - make it findable
# - do not force a phone call if an online method is legally required/available
# - avoid retention dark patterns
# - confirm successful cancellation
# - state the effective date
# - provide evidence / email confirmation
#
# =========================
# 20. CONSUMER PROTECTION / DARK PATTERNS
# =========================
#
# Review for:
# - false scarcity
# - fake countdowns
# - fake reviews
# - hidden fees
# - drip pricing
# - misleading reference prices
# - fake endorsements
# - disguised ads
# - forced continuity
# - pre-selected paid extras
# - misleading cancellation
# - misleading social proof
#
# Keep evidence for objective claims:
#   "No. 1"
#   "best"
#   "fastest"
#   "award-winning"
#   "save 50%"
#   "only 2 left"
#
# =========================
# 21. ADVERTISING — ASA / CAP
# =========================
#
# The CAP Code can apply to advertising on a company's own website.
# It does not mean every sentence on a company website is an ad;
# classify promotional content carefully.
#
# Review:
# - truthfulness
# - substantiation
# - identifiable advertising
# - pricing
# - comparative claims
# - environmental claims
# - health claims
# - testimonials
# - influencer/affiliate content
# - children
# - direct marketing
#
# Do not rely on "it's our own website so ASA doesn't apply".
#
# =========================
# 22. REVIEWS / TESTIMONIALS
# =========================
#
# If the company displays reviews:
# - do not create fake reviews
# - do not suppress genuine negative reviews in a misleading way
# - explain verification methods where claimed
# - disclose incentives
# - moderate consistently
# - avoid fabricating customer quotes
#
# =========================
# 23. AFFILIATE / SPONSORED CONTENT
# =========================
#
# Label commercial relationships clearly.
# Ensure the audience can understand the commercial nature of the content.
# Keep records of advertiser/affiliate relationships.
#
# =========================
# 24. COPYRIGHT / IMAGE RIGHTS
# =========================
#
# For every asset, establish rights:
# - own
# - licensed
# - public domain
# - valid open licence
# - commissioned with appropriate rights
#
# Track:
# - copyright owner
# - licence
# - territory
# - duration
# - media
# - attribution
# - restrictions
#
# Never scrape Google Images and publish by default.
#
# =========================
# 25. TRADE MARKS / BRAND USAGE
# =========================
#
# Check:
# - company name
# - logos
# - product names
# - competitor references
# - partner logos
# - endorsements
#
# Do not imply official partnership or endorsement without a factual basis.
#
# =========================
# 26. TEXT / EDITORIAL / DEFAMATION
# =========================
#
# For claims about people or companies:
# - separate fact from opinion
# - substantiate factual claims
# - avoid defamatory statements
# - retain source evidence
# - review user-submitted accusations carefully
#
# =========================
# 27. AI-GENERATED CONTENT
# =========================
#
# When using AI for website content or customer decisions:
# - verify factual accuracy
# - avoid fabricated testimonials
# - verify image rights
# - check personal-data inputs
# - document high-risk AI processing
# - disclose AI use where legally/ethically appropriate
# - do not invent certifications
# - do not invent statistics
#
# If AI makes decisions about customers, activate the automated decision-making module.
#
# =========================
# 28. USER-GENERATED CONTENT / PLATFORM
# =========================
#
# Activate only if users can:
# - upload content
# - post comments
# - message others
# - create public profiles
# - sell to each other
# - publish listings
# - share content beyond the individual
#
# Then assess:
# - Online Safety Act
# - copyright / infringement procedures
# - moderation
# - reporting
# - appeals
# - child safety
# - privacy
# - terms
# - illegal-content handling
#
# The Online Safety Act applies to regulated user-to-user/search services with
# the relevant UK links and scope conditions; it is not a blanket obligation for
# every brochure website.
#
# =========================
# 29. MARKETPLACE
# =========================
#
# Activate for third-party sellers.
# Review:
# - trader verification
# - seller identity
# - seller disclosures
# - ranking transparency where required
# - reviews
# - prohibited goods
# - complaints
# - payments
# - refunds
# - illegal content
# - consumer protection
#
# =========================
# 30. BOOKINGS / APPOINTMENTS
# =========================
#
# For booking websites:
# - price
# - duration
# - availability
# - cancellation
# - deposit
# - no-show fee
# - recurring appointment
# - provider identity
# - confirmation
# - reminders
#
# If the service is consumer-facing and booked at a distance, review applicable
# distance-contract rules.
#
# =========================
# 31. B2B-ONLY WEBSITES
# =========================
#
# Do not automatically apply consumer-only rights.
# But verify:
# - business identity
# - contract terms
# - payment terms
# - VAT
# - intellectual-property terms
# - confidentiality
# - security
# - data protection
# - marketing
#
# =========================
# 32. UK NATIONS / LOCAL LAW
# =========================
#
# Do not pretend "UK law" is always uniform.
# Check whether the feature is affected by:
# - England & Wales
# - Scotland
# - Northern Ireland
#
# Particular areas can differ:
# - consumer / contract procedures
# - property
# - courts / jurisdiction
# - professional regulation
# - local licensing
#
# =========================
# 33. TAX / VAT
# =========================
#
# If prices are shown to UK consumers:
# - determine whether prices must include VAT
# - identify registration status
# - ensure checkout calculations match
#
# If selling internationally:
# - check destination VAT
# - digital-service rules
# - import/export
# - duties
# - place-of-supply
#
# Never fabricate VAT numbers.
#
# =========================
# 34. PAYMENTS
# =========================
#
# If accepting payments:
# - use a reputable payment processor
# - minimise card-data exposure
# - do not store raw card data unless genuinely authorised and designed for it
# - review PCI DSS scope
# - secure webhooks
# - verify payment server-side
# - prevent price tampering
# - prevent replay attacks
# - do not trust client-side "paid" flags
#
# =========================
# 35. CUSTOMER ACCOUNTS
# =========================
#
# Implement:
# - secure authentication
# - password hashing
# - MFA option where appropriate
# - session expiration
# - logout invalidation
# - account recovery
# - anti-enumeration protections
# - brute-force protection
# - access controls
# - data export/deletion workflow
#
# =========================
# 36. EMAIL / COMMUNICATIONS
# =========================
#
# Service emails:
# - account confirmation
# - invoice
# - security alert
# - delivery
# - booking
#
# Marketing emails:
# - separate legal analysis
# - unsubscribe
# - correct sender identity
# - records
#
# Do not turn transactional emails into hidden marketing without analysis.
#
# =========================
# 37. LOGGING / RETENTION
# =========================
#
# Define retention for:
# - contact requests
# - analytics data
# - customer accounts
# - orders
# - invoices
# - marketing consent records
# - security logs
# - support conversations
#
# Never use "keep forever" as the default.
#
# =========================
# 38. DOCUMENT GENERATION
# =========================
#
# If generating legal pages, create:
#   /legal/privacy
#   /legal/cookies
#   /legal/terms
#   /legal/refunds
#   /legal/cancellation
#   /legal/accessibility
# as applicable.
#
# Each must be generated from actual project facts.
#
# Required placeholders should be obvious:
#   [LEGAL_COMPANY_NAME]
#   [REGISTERED_OFFICE]
#   [COMPANY_NUMBER]
#   [VAT_NUMBER]
#   [CONTACT_EMAIL]
#
# NEVER invent placeholder values that look real.
#
# =========================
# 39. COOKIE NOTICE IMPLEMENTATION SPEC
# =========================
#
# Create a consent state model:
#
#   necessary: always allowed where law permits
#   preferences: off by default unless chosen
#   analytics: off by default unless lawful alternative / consent
#   marketing: off by default unless lawful alternative / consent
#
# Store:
# - consent id
# - version
# - timestamp
# - categories
# - notice version
#
# Provide:
#   "Change cookie choices"
#
# Ensure withdrawn consent stops further non-essential activation as technically feasible.
#
# =========================
# 40. LEGAL-LINK INTEGRITY
# =========================
#
# Test:
# - privacy link returns 200
# - cookie settings open
# - terms link works
# - cancellation / refund pages work
# - links are readable on mobile
# - no dead links
# - legal pages are indexable/noindex deliberately, not accidentally
#
# =========================
# 41. SEO + LEGAL
# =========================
#
# SEO must not create misleading claims.
# Avoid:
# - doorway pages
# - fake local addresses
# - fake reviews
# - fabricated schema markup
# - false organisation data
# - fake ratings
#
# Structured data must match visible content.
#
# =========================
# 42. SCHEMA / RICH RESULTS
# =========================
#
# For Organization / LocalBusiness / Product / Review schema:
# - use real values
# - never invent ratings
# - never invent reviews
# - ensure legal company name is accurate
# - ensure address and telephone are real
#
# =========================
# 43. SERVER / INFRASTRUCTURE
# =========================
#
# Review:
# - hosting location
# - backups
# - DNS
# - email provider
# - CDN
# - WAF
# - object storage
# - logging
# - monitoring
#
# Document every system touching personal data.
#
# =========================
# 44. DEVELOPMENT DEPENDENCIES
# =========================
#
# Inventory:
# - npm packages
# - JS bundles
# - fonts
# - icon packages
# - analytics SDKs
# - CSS frameworks
# - CAPTCHA
# - UI components
#
# Check:
# - licence
# - known vulnerabilities
# - data collection
# - network calls
#
# =========================
# 45. OPEN-SOURCE LICENSING
# =========================
#
# For copied code/assets:
# - identify licence
# - preserve required notices
# - satisfy attribution requirements
# - assess copyleft obligations
#
# Never delete licence files just to make the project look cleaner.
#
# =========================
# 46. SECURITY HEADERS BASELINE
# =========================
#
# Consider, as appropriate:
#   Strict-Transport-Security
#   Content-Security-Policy
#   X-Content-Type-Options
#   Referrer-Policy
#   Permissions-Policy
#   frame-ancestors / clickjacking protection
#
# Do not blindly copy a CSP that breaks the site.
# Generate it from actual dependencies.
#
# =========================
# 47. ACCESSIBILITY TEST MATRIX
# =========================
#
# Test:
# - keyboard only
# - screen reader
# - 200% zoom
# - 400% zoom where practical
# - mobile
# - focus order
# - forms
# - errors
# - menus
# - modals
# - animations
# - video captions
#
# Automated testing is not sufficient by itself.
#
# =========================
# 48. FORM SECURITY TEST MATRIX
# =========================
#
# Attempt:
# - invalid email
# - empty required field
# - oversized payload
# - HTML injection
# - script injection
# - SQL injection patterns
# - CSRF
# - spam
# - duplicate submission
# - race conditions
#
# =========================
# 49. PAYMENT TEST MATRIX
# =========================
#
# Attempt:
# - altered price
# - altered product id
# - duplicate webhook
# - failed payment
# - refund
# - partial refund
# - chargeback notification
# - delayed webhook
# - tampered success URL
#
# Trust only server-verified payment events.
#
# =========================
# 50. COMPLIANCE AUTOMATION
# =========================
#
# Build scripts where useful:
#
#   npm run compliance:links
#   npm run compliance:third-party
#   npm run compliance:cookies
#   npm run compliance:headers
#   npm run compliance:accessibility
#   npm run compliance:privacy
#   npm run compliance:all
#
# The scripts should output machine-readable JSON and human-readable Markdown.
#
# Example artifact:
#   reports/uk-compliance-report.json
#
# =========================
# 51. THIRD-PARTY NETWORK SCAN
# =========================
#
# On a production-like build:
# 1. open homepage in fresh context
# 2. record network requests
# 3. classify each external host
# 4. repeat without consent
# 5. accept analytics
# 6. accept marketing
# 7. revoke
# 8. diff requests
#
# Any unknown external domain = FAIL until classified.
#
# =========================
# 52. PRIVACY NOTICE ↔ CODE CONSISTENCY
# =========================
#
# Every material processing statement in privacy notice should be traceable to:
# - code
# - backend config
# - vendor contract
# - operational process
#
# Every known processing activity should have a documentation entry.
#
# Examples of contradictions that must be caught:
# - notice says "no analytics"; code loads analytics
# - notice says "data stored in UK"; vendor stores it elsewhere
# - notice says "no marketing"; form enables promotional messaging
# - notice says "session cookies only"; localStorage stores identifiers
#
# =========================
# 53. LEGAL PAGE CONTENT RULES
# =========================
#
# Legal pages must:
# - use plain language where practical
# - have correct company identity
# - state effective date / last updated date
# - avoid fake statutory citations
# - avoid promises stronger than operations
# - not claim "fully GDPR compliant" without an audit basis
#
# =========================
# 54. TERMS / CONTRACTS
# =========================
#
# Do not use copied template terms without adaptation.
#
# Verify:
# - parties
# - scope
# - payment
# - delivery
# - cancellation
# - refunds
# - liability
# - IP
# - confidentiality
# - acceptable use
# - suspension/termination
# - governing law
# - jurisdiction
# - complaint handling
#
# For consumers, test terms against unfair-terms rules.
#
# =========================
# 55. PROFESSIONAL / REGULATED SECTOR MODULE
# =========================
#
# Activate based on industry.
#
# Potential examples:
# - financial services / FCA
# - insurance
# - healthcare
# - legal services
# - education
# - gambling
# - alcohol
# - food
# - travel
# - real estate
# - employment / recruitment
# - telecoms
# - children's services
#
# Never apply a sector module unless scope is established.
#
# =========================
# 56. FINANCIAL SERVICES MODULE
# =========================
#
# If FCA-regulated or otherwise financial:
# - verify FCA permissions
# - regulated-status wording
# - financial promotions
# - consumer duty
# - complaints
# - risk warnings
# - approval of promotions
# - record keeping
#
# Do not improvise financial-regulatory statements.
#
# =========================
# 57. HEALTHCARE MODULE
# =========================
#
# Review:
# - professional regulation
# - health claims
# - patient confidentiality
# - special-category data
# - medical-device advertising
# - medicines advertising
# - appointment processing
#
# =========================
# 58. FOOD MODULE
# =========================
#
# Online food sellers may need:
# - food-business registration
# - allergen information
# - mandatory product information
# - delivery conditions
# - distance-selling rules
#
# GOV.UK explicitly confirms online food sellers must address pre-sale
# information and allergen requirements.
#
# =========================
# 59. CHILDREN / FAMILY MODULE
# =========================
#
# Assess:
# - age range
# - data collection
# - profiling
# - direct marketing
# - design code / children's privacy risk
# - harmful content
#
# Use the current ICO guidance, not a pre-2025 checklist.
#
# =========================
# 60. ONLINE SAFETY MODULE
# =========================
#
# Activate if the service is a regulated user-to-user or search service.
# Determine UK link / target market / material risk scope.
#
# Review:
# - illegal-content risk assessment
# - child safety duties
# - content moderation
# - user reporting
# - complaints
# - record keeping
# - terms enforcement
# - OFCOM interaction
#
# Do not apply these duties to an ordinary brochure site merely because it has a contact form.
#
# =========================
# 61. INTERNATIONAL WEBSITE
# =========================
#
# If the company targets EU/EEA consumers, do not stop at UK law.
# Activate a separate EU module.
#
# Possible extra modules:
# - EU GDPR
# - EU consumer law
# - DSA
# - accessibility legislation
# - VAT
#
# Likewise, if targeting US consumers, use a dedicated US module.
#
# =========================
# 62. LEGAL TEXT VERSIONING
# =========================
#
# Every change to:
# - privacy notice
# - cookie notice
# - terms
# - cancellation
# - accessibility notice
# should create a version identifier.
#
# Record:
# - date
# - reason
# - affected systems
# - whether customer consent must be renewed
#
# =========================
# 63. COOKIE / CONSENT VERSIONING
# =========================
#
# When purposes/providers change materially:
# - update notice
# - update consent configuration
# - evaluate whether existing consent remains valid
#
# =========================
# 64. COMPLIANCE EVIDENCE
# =========================
#
# Keep evidence of:
# - consent logs
# - privacy notice versions
# - vendor agreements
# - data maps
# - transfer assessments
# - security tests
# - accessibility tests
# - content-claim substantiation
# - licences
# - company details
# - regulator registrations
#
# =========================
# 65. PRE-LAUNCH LEGAL GATE
# =========================
#
# DO NOT PASS if:
# - company identity is missing/incorrect
# - privacy notice is missing where required
# - cookies/trackers are uncontrolled
# - unknown third parties exist
# - payment obligation is unclear
# - mandatory consumer information is missing
# - required cancellation flow is missing
# - marketing consent has no evidence
# - major security vulnerabilities exist
# - accessibility failures materially affect the intended service
# - claims have no substantiation
#
# PASS only when:
# - every applicable module is PASS or documented NEEDS LEGAL REVIEW
# - all FAIL items resolved
# - all assumptions recorded
#
# =========================
# 66. CLAUDE WORKFLOW
# =========================
#
# When asked to build/fix a UK company website:
#
# STEP 1 — inspect repository
# STEP 2 — identify site class
# STEP 3 — inspect package.json / dependencies
# STEP 4 — scan external domains
# STEP 5 — inspect forms / tracking / auth / checkout
# STEP 6 — build compliance manifest
# STEP 7 — implement core technical protections
# STEP 8 — implement legal-page placeholders
# STEP 9 — implement consent / privacy controls
# STEP 10 — test accessibility
# STEP 11 — test security
# STEP 12 — test legal links
# STEP 13 — run compliance report
# STEP 14 — report unresolved legal questions
#
# =========================
# 67. CLAUDE CODING RULES
# =========================
#
# - Never silently add analytics.
# - Never silently add a marketing pixel.
# - Never silently embed third-party content.
# - Never hard-code fake company data.
# - Never write fake reviews.
# - Never fabricate certifications.
# - Never fabricate legal wording as fact.
# - Never disable security controls to "make the demo work" without flagging it.
# - Never store secrets in frontend code.
# - Never trust client-only payment success.
# - Never pre-check optional marketing consent.
# - Never call an optional cookie "necessary" without analysis.
# - Never use an online privacy-policy generator output blindly.
#
# =========================
# 68. REPORT FORMAT
# =========================
#
# At the end, produce:
#
# UK WEBSITE COMPLIANCE REPORT
# ----------------------------
# Date:
# Jurisdiction:
# Company:
# Site class:
# Customer type:
#
# CORE
# [PASS/FAIL/REVIEW] Company information
# [PASS/FAIL/REVIEW] Privacy
# [PASS/FAIL/REVIEW] PECR / storage-access tech
# [PASS/FAIL/REVIEW] Security
# [PASS/FAIL/REVIEW] Accessibility
#
# CONDITIONAL
# [N/A/PASS/FAIL/REVIEW] Ecommerce
# [N/A/PASS/FAIL/REVIEW] Cancellation
# [N/A/PASS/FAIL/REVIEW] Subscription
# [N/A/PASS/FAIL/REVIEW] Marketing
# [N/A/PASS/FAIL/REVIEW] UGC / Online Safety
# [N/A/PASS/FAIL/REVIEW] Sector regulation
#
# THIRD PARTIES
# count:
# unknown:
#
# OPEN LEGAL QUESTIONS
# ...
#
# TECHNICAL FAILURES
# ...
#
# LAUNCH STATUS
#   NO-LAUNCH
#   CONDITIONAL
#   READY-FOR-LEGAL-REVIEW
#   READY-FOR-LAUNCH
#
# Never use "100% legal".
#
# =========================
# 69. CURRENT-2026 VERIFICATION CHECKLIST
# =========================
#
# Before finalising any project, verify all current changes since this file's
# baseline date from official sources.
#
# REQUIRED:
# [ ] ICO DUAA 2025 guidance current
# [ ] ICO Storage and Access Technologies guidance current
# [ ] PECR current text
# [ ] UK GDPR current text / amendments
# [ ] DPA 2018 current text / amendments
# [ ] Companies Act / company website information current
# [ ] Electronic Commerce Regulations current
# [ ] Consumer Contracts rules current
# [ ] Consumer Rights Act current
# [ ] DMCC Act commencement status current
# [ ] ASA/CAP current code / guidance
# [ ] Online Safety scope / Ofcom requirements current, if applicable
# [ ] Equality Act / applicable accessibility law current
# [ ] sector regulator requirements current, if applicable
#
# =========================
# 70. SOURCE SNAPSHOT — 11 SEPTEMBER 2026
# =========================
#
# Key current official references used to build this skill:
#
# 1) ICO — DUAA 2025, organisations:
#    https://ico.org.uk/about-the-ico/what-we-do/legislation-we-cover/
#    data-use-and-access-act-2025/the-data-use-and-access-act-2025-what-does-it-mean-for-organisations/
#    ICO update: 19 June 2026 — all data protection provisions in force.
#
# 2) ICO — Storage and Access Technologies:
#    https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-
#    communications/guidance-on-the-use-of-storage-and-access-technologies/
#    Final guidance: 29 April 2026.
#    Covers cookies, pixels, link decoration, fingerprinting, web storage, scripts/tags
#    and related technologies under PECR and, where personal data is involved, UK GDPR.
#
# 3) ICO — Electronic and telephone marketing:
#    https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-
#    communications/guide-to-pecr/electronic-and-telephone-marketing/
#
# 4) ICO — Electronic mail marketing:
#    https://ico.org.uk/for-organisations/direct-marketing-and-privacy-and-electronic-
#    communications/guidance-on-direct-marketing-using-electronic-mail/
#    Updated 28 April 2026, including DUAA changes to charitable soft opt-in.
#
# 5) GOV.UK — Online and distance selling:
#    https://www.gov.uk/online-and-distance-selling-for-businesses
#    and /online-selling
#
# 6) GOV.UK — Returns / refunds:
#    https://www.gov.uk/accepting-returns-and-giving-refunds
#
# 7) UK legislation:
#    https://www.legislation.gov.uk/
#
# 8) ASA / CAP — own websites:
#    https://www.asa.org.uk/advice-online/remit-own-websites.html
#    Current guidance crawled in 2026; CAP Code can cover advertising on a company's
#    own website.
#
# 9) ASA / CAP — company names and URLs:
#    https://www.asa.org.uk/advice-online/company-names-and-urls.html
#    Published 31 July 2026.
#
# =========================
# 71. FINAL IMPLEMENTATION DIRECTIVE
# =========================
#
# Treat this file as a decision engine, not a static list.
#
# For every feature:
#   1. identify the feature
#   2. identify affected people
#   3. identify jurisdictions
#   4. identify applicable law
#   5. verify current official source
#   6. classify requirement
#   7. implement technical control
#   8. document legal basis
#   9. test
#   10. record PASS / FAIL / REVIEW / N/A
#
# If a legal rule is uncertain, say exactly what is uncertain.
# Do not fill gaps with guesses.
#
# END OF SKILL
