# Tier1: HubSpot Breeze AI Audit Checklist (2026)

This checklist is used to verify the integrity of HubSpot's Outcome-Based Billing and Lead Status logic.

### 1. Billing Integrity (Outcome Accuracy Check)
- [ ] Export 'Chat Conversations' with the `hs_ct_agent_resolution_status` property.
- [ ] Cross-reference 'RESOLVED' outcomes against 'User Exit Intent' (detecting abandonment vs. success).
- [ ] Identify 'Resolution Loops' (multiple charges for a single user issue).

### 2. July 13 Data Lockdown Readiness
- [ ] Audit `hs_customer_agent_lead_status` for AI-driven miscategorization.
- [ ] Verify lead logic before property becomes System-Managed (Read-Only) on July 13, 2026.

### 3. Credit Consumption Recovery
- [ ] Compare 'Breeze' credit spend against actual CRM record creation.
- [ ] Flag 'Ghost Resolutions' (charges incurred with zero data updates to the CRM).
