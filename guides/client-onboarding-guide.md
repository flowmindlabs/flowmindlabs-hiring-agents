# FlowMind Labs — Client Onboarding Guide

**For FlowMind Labs team and partners. Complete this checklist for every new client.**

---

## Phase 1: Pre-Sale (Before signing)

- [ ] Understand client's business — type, size, primary problem to solve
- [ ] Recommend the right BSP: Chakra Chat (budget), AiSensy (leads), Interakt (mid), Wati (enterprise)
- [ ] Confirm client has or can get a dedicated WhatsApp Business number
- [ ] Show demo workflow — screen share or loom video
- [ ] Send pricing proposal with setup fee + monthly plan
- [ ] Send Client Security Agreement (`guides/client-security-agreement.md` in n8n-workflows repo)

---

## Phase 2: Onboarding (After payment)

### 2.1 Collect from client
- [ ] Business name, address, working hours
- [ ] WhatsApp Business number (dedicated, not personal)
- [ ] BSP API key (or help them sign up)
- [ ] FAQ content — top 20 questions + answers
- [ ] Booking slots / availability (if booking agent)
- [ ] Airtable access or create a base for them
- [ ] Logo + brand colors (for any email templates)

### 2.2 Setup (your side)
- [ ] Import workflow JSON into n8n
- [ ] Fill `BUSINESS_CONFIG` / `FAQ_CONFIG` / `LEAD_CONFIG` node with client details
- [ ] Add all credentials to n8n credential vault (never in workflow JSON)
- [ ] Set webhook URL in BSP dashboard
- [ ] Activate workflow
- [ ] Run 5 test messages covering: normal query, booking/lead, edge case, escalation trigger, error path

### 2.3 Handover call (30 min with client)
- [ ] Show client how to view Airtable records
- [ ] Show client how escalation alerts arrive (WhatsApp/email)
- [ ] Explain what to do if bot stops responding (contact hello@flowmindlabs.co)
- [ ] Share this doc: what we're responsible for vs what they are
- [ ] Confirm they've read and signed the Client Security Agreement

---

## Phase 3: Go Live

- [ ] Client sends first real customer message — verify end-to-end
- [ ] Monitor n8n Executions tab for first 24 hours
- [ ] Check Airtable records populating correctly
- [ ] Send client a "you're live!" WhatsApp message with quick-reference card:
  - How to view bookings/leads: [Airtable link]
  - What escalation alerts look like
  - Support contact: hello@flowmindlabs.co

---

## Phase 4: Ongoing (Monthly)

- [ ] Test workflow with sample message
- [ ] Check API key expiry — rotate if expiring within 30 days
- [ ] Review n8n execution errors from past month
- [ ] Check BSP account standing
- [ ] Review usage vs plan limits — upsell if at 80%+
- [ ] Send client monthly summary (optional, paid add-on)

---

## BSP Quick Reference

| BSP | Sign-up | API key location | Webhook setting |
|---|---|---|---|
| Chakra Chat | chakra.chat | Dashboard → API Keys | Dashboard → Webhooks |
| AiSensy | aisensy.com | Settings → API | Settings → Webhooks |
| Interakt | interakt.shop | Settings → API Key | Settings → Webhooks |
| Wati | wati.io | Settings → API | Settings → Webhooks |

---

## Support Contacts

- FlowMind Labs: hello@flowmindlabs.co
- Anthropic status: status.anthropic.com
- n8n docs: docs.n8n.io
- Troubleshooting: see `guides/troubleshooting-runbook.md`

---

*FlowMind Labs | hello@flowmindlabs.co | flowmindlabs.co*
