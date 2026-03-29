# Access to Safety

**The most comprehensive community safety navigation tool on the planet.**

*Part of the [Access To](https://cotrackpro.github.io/access-to/) project family — open-source Claude skills for human rights infrastructure.*

[![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Pillar: Safety](https://img.shields.io/badge/Pillar-Safety-red.svg)](#)
[![Region: St. Louis County MO](https://img.shields.io/badge/Region-STL%20County%20MO-blue.svg)](#)

---

## What Is This?

Access to Safety is an AI skill (designed for [Claude](https://claude.ai)) that navigates **every dimension of community safety** — from crisis response and domestic violence to cyberstalking and disaster preparedness. It ships with St. Louis County, Missouri as the reference implementation and is designed to be forked and customized for any region on Earth.

**This is not a chatbot.** It's a structured knowledge system that:
- Routes any safety concern to the right resources
- Generates personalized safety plans
- Produces court-ready incident documentation
- Provides evidence-quality risk assessments
- Covers 8 safety domains with 100+ subtopics
- Includes every relevant hotline, statute, and procedure
- Maintains trauma-informed, child-centered, privacy-first tone at all times

---

## The 8 Safety Domains

| # | Domain | What It Covers |
|---|--------|---------------|
| 1 | **Crisis Response** | 911, 988, crisis lines, mobile crisis teams, co-responder models, crisis stabilization |
| 2 | **Violence & Abuse** | Domestic violence, child abuse/neglect, sexual violence, elder abuse, human trafficking, stalking |
| 3 | **Community Safety** | Gun violence, community violence intervention (CVI), hate crimes, school safety, active threats |
| 4 | **Legal Protection** | Protective orders, victim rights, crime victim compensation, VOCA, mandatory reporting |
| 5 | **Behavioral Health Crisis** | 988 system, psychiatric holds, suicide prevention, overdose response, naloxone, MAT |
| 6 | **Environmental Safety** | Disaster preparedness, housing safety, lead/mold/code violations, workplace safety |
| 7 | **Digital & Tech Safety** | Cyberstalking, spyware, AirTag tracking, doxxing, NCII/revenge porn, sextortion, CSAM reporting |
| 8 | **Vulnerable Populations** | LGBTQ+, disability, immigration (U/T-visa), refugee, veteran, unhoused, youth aging out, tribal |

Plus **4 cross-cutting tools**: Safety Plan Builder, Incident Documentation, Resource Directory, and a Region Customization Guide.

---

## Quick Start

### Use as a Claude Skill

1. Download this repository
2. Add the `access-to-safety/` folder to your Claude skill directory
3. Claude will automatically route safety-related questions to the appropriate domain

### Fork for Your Region

1. Fork this repo
2. Read `templates/customization-guide.md`
3. Replace St. Louis County data in each pod file with your local resources
4. Validate all phone numbers and addresses
5. Submit a PR to share your region with the community

See the full [Customization Guide](templates/customization-guide.md).

---

## File Structure

```
access-to-safety/
├── README.md                                    ← You are here
├── SKILL.md                                     ← Main skill file (routing + principles)
├── references/
│   ├── crisis-response/pod.md                   ← Pod 1: 911, crisis lines, mobile crisis
│   ├── violence-abuse/pod.md                    ← Pod 2: DV, child abuse, sexual violence, trafficking
│   ├── community-safety/pod.md                  ← Pod 3: Gun violence, CVI, hate crimes, schools
│   ├── legal-protection/pod.md                  ← Pod 4: Protective orders, victim rights, reporting
│   ├── behavioral-health-crisis/pod.md          ← Pod 5: 988, psychiatric holds, overdose, naloxone
│   ├── environmental-safety/pod.md              ← Pod 6: Disasters, housing, workplace, hazards
│   ├── digital-safety/pod.md                    ← Pod 7: Cyberstalking, spyware, doxxing, CSAM
│   └── vulnerable-populations/pod.md            ← Pod 8: LGBTQ+, disability, immigration, veterans
├── templates/
│   ├── safety-plan.md                           ← Personalized safety plan builder
│   ├── incident-log.md                          ← Evidence-quality incident documentation
│   ├── resource-directory.md                    ← Blank directory template for any region
│   └── customization-guide.md                   ← How to fork for your region
└── schemas/
    ├── resource-entry.json                      ← JSON schema: single resource entry
    ├── safety-assessment.json                   ← JSON schema: risk/needs assessment
    └── incident-record.json                     ← JSON schema: court-ready incident log
```

---

## Design Principles

1. **Safety first.** Immediate danger → emergency numbers before anything else.
2. **Trauma-informed.** Never blame. Never interrogate. Validate. Empower choice.
3. **Child-centered.** Children's safety and wellbeing take priority.
4. **Culturally responsive.** Acknowledge barriers: language, immigration, disability, identity.
5. **Privacy-first.** Warn about digital footprints. Never store PII.
6. **Empowerment over rescue.** Provide information and options. The person decides.
7. **Plain language.** 8th grade reading level for user-facing content.
8. **Accurate sourcing.** Real hotlines, real agencies, real statutes. Never fabricate.

---

## The Access To Family

| Pillar | Repository | Focus |
|--------|-----------|-------|
| **Justice** | access-to-justice | Expungement, legal aid, court navigation |
| **Education** | access-to-education | K-12 standards, special education, teacher support |
| **Housing** | access-to-housing | Tenant rights, fair housing, homelessness |
| **Services** | access-to-services | Social services navigation, benefits, intake |
| **Peace** | access-to-peace | Conflict resolution, restorative justice, mediation |
| **Safety** | **access-to-safety** | **Crisis response, violence prevention, protection** |

---

## Contributing

We welcome contributions from:

- **Domestic violence advocates** who know the resource landscape
- **Legal aid attorneys** who know protective order procedures
- **Crisis counselors** who work the hotlines
- **Emergency managers** who coordinate disaster response
- **Social workers** who navigate these systems daily
- **Survivors** who know what information they needed and couldn't find
- **Developers** who want to build tools on top of these schemas
- **Researchers** who study safety system effectiveness

### How to Contribute

1. **Add your region:** Fork, localize, submit a PR
2. **Fix a resource:** Found an outdated number? Open an issue or PR
3. **Add a subtopic:** See something we missed? Propose an addition
4. **Improve language:** Help us be clearer, more accessible, more inclusive
5. **Build on the schemas:** Create apps, dashboards, or tools using our JSON schemas

### Content Guidelines

- Plain language (≤ 8th grade reading level for user-facing content)
- Trauma-informed tone (no blaming, no jargon, empowerment over rescue)
- Factual and verifiable (cite sources, verify numbers)
- Privacy-conscious (no confidential addresses, no PII)
- Inclusive (consider all populations served)

---

## Important Notes

- **This is not legal advice.** This is educational safety information.
- **This is not a clinical tool.** The safety assessment is an information-gathering framework, not a validated clinical instrument.
- **This is not a substitute for 911.** If someone is in immediate danger, call 911.
- **Resources change.** Phone numbers, addresses, and services should be verified regularly.
- **Laws vary.** State statutes referenced are Missouri-specific unless noted. Fork and update for your jurisdiction.

---

## License

MIT — fork freely, customize for your community, share what you build.

---

## Emergency Numbers

If you or someone you know is in immediate danger:

| Resource | Contact |
|----------|---------|
| **Emergency** | **911** |
| **Suicide & Crisis** | **988** (call or text) |
| **Domestic Violence** | **1-800-799-7233** |
| **Child Abuse** | **1-800-422-4453** |
| **Sexual Assault** | **1-800-656-4673** |
| **Human Trafficking** | **1-888-373-7888** |
| **Poison Control** | **1-800-222-1222** |
| **Crisis Text Line** | Text **HOME** to **741741** |

---

*Built with care by the [CoTrackPro](https://cotrackpro.com) community. Because everyone deserves to know how to be safe.*
