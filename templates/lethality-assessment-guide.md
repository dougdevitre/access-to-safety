# Lethality Assessment Protocol (LAP) — Advocate Guide

> **AI Instructions:** When an advocate asks for help with a lethality assessment, danger
> assessment, or risk screening, walk them through this protocol step by step. This is a
> guide for using validated lethality screening tools — it is NOT a substitute for the
> validated instruments themselves (which are copyrighted). Always remind advocates that
> this guide supports — but does not replace — their professional training. If the survivor
> screens in as high danger, immediately shift to safety planning and connect them with the
> appropriate crisis resources. Never assign a "score" or render a clinical opinion — the
> advocate's trained judgment is what matters.

---

## What This Guide Is

This is an advocate-facing reference for conducting lethality screenings in domestic
violence cases. It aligns with the **Maryland Model Lethality Assessment Protocol**
(developed by the Maryland Network Against Domestic Violence) and the **Danger Assessment**
(developed by Dr. Jacquelyn Campbell, Johns Hopkins University).

**This guide does NOT replace:**
- Formal LAP training (required before administering the screen)
- The copyrighted Danger Assessment instrument (available at dangerassessment.org)
- Clinical judgment or professional supervision

**This guide DOES provide:**
- A structured workflow for advocates who are already LAP-trained
- Quick-reference risk factor lists aligned with validated research
- Documentation guidance for assessment results
- Decision trees for high-danger referrals
- Language suggestions for discussing lethality with survivors

---

## When to Use a Lethality Screen

| Situation | Action |
|-----------|--------|
| First contact with a new client experiencing IPV | Conduct screening |
| Survivor reports a recent incident of violence | Conduct or update screening |
| Survivor is planning to leave or has recently left | Conduct or update screening (leaving is the highest-risk period) |
| Significant change in abuser behavior (escalation, weapons, threats to kill) | Update screening immediately |
| Law enforcement calls in from the scene | Guide officer through the screen questions by phone |
| Routine follow-up with ongoing client | Reassess if 90+ days since last screen or if situation has changed |

---

## The 11-Question Lethality Screen — Reference Framework

> **Note:** The exact wording of the validated Lethality Screen for First Responders is
> copyrighted by the Maryland Network Against Domestic Violence. The following are the
> general risk factor domains that the screen covers. Use the validated instrument in
> practice.

### High-Danger Indicators (any single "yes" = high danger)

These factors are individually predictive of lethal or near-lethal violence:

| # | Risk Factor Domain | Why It Matters |
|---|-------------------|----------------|
| 1 | **Abuser has used a weapon against survivor or threatened with a weapon** | Weapon involvement is the single strongest predictor of DV homicide |
| 2 | **Abuser has threatened to kill the survivor** | Direct threats to kill are taken at face value in lethality research |
| 3 | **Survivor believes the abuser is capable of killing them** | Survivor perception of danger is highly predictive — trust their instinct |
| 4 | **Abuser has choked, strangled, or "choked" the survivor** | Non-fatal strangulation increases homicide risk by 750% (Glass et al., 2008) |

### Escalation Indicators (3+ "yes" answers across these = high danger)

| # | Risk Factor Domain | Why It Matters |
|---|-------------------|----------------|
| 5 | **Abuser has access to a gun** | Firearms are used in 52% of DV homicides |
| 6 | **Abuser has forced sexual acts** | Sexual violence within IPV strongly predicts escalation to lethal violence |
| 7 | **Violence is increasing in frequency or severity** | Escalation pattern is a core predictor |
| 8 | **Abuser uses illegal drugs or heavily drinks** | Substance use lowers inhibition and correlates with lethal violence |
| 9 | **Abuser has threatened or attempted suicide** | Murder-suicide is a distinct DV homicide pattern |
| 10 | **Survivor is leaving, has left, or is planning to leave** | Separation is the highest-risk period — 75% of DV homicides occur at or after separation |
| 11 | **Abuser is constantly jealous or controls most of the survivor's daily activities** | Coercive control and obsessive jealousy are core lethality predictors |

---

## Conducting the Screen — Advocate Workflow

### Before the Screen

1. **Ensure immediate safety.** If the survivor is in danger right now, address that first (call 911, create physical distance, move to a safe space).
2. **Explain what you are doing and why.** Use plain language:
   > *"I'm going to ask you some questions about your situation. These questions help us
   > understand if you are in a particularly dangerous situation so we can make sure you
   > get the right kind of help. There are no wrong answers. You can skip any question you
   > are not comfortable answering."*
3. **Get verbal consent.** The survivor should understand that:
   - The screen is voluntary
   - The results will be used to inform safety planning, not to make decisions for them
   - The information is confidential within normal limits (explain any mandatory reporting obligations)
4. **Use a private, safe space.** Never conduct a screen where the abuser may overhear.

### During the Screen

- **Ask each question in the survivor's own language.** If using an interpreter, ensure the interpreter is trained in DV dynamics (not a family member, not a community member who might know the abuser).
- **Do not rush.** Let the survivor take their time. These are difficult questions.
- **Do not react with alarm.** A calm, steady presence helps the survivor stay regulated. Even if every answer is "yes," your demeanor should stay grounded.
- **Take notes using non-identifying shorthand.** Do not write the survivor's name on the screening form if there is any risk the abuser could access it.
- **Ask follow-up questions when needed.** If the survivor says "yes" to strangulation, ask:
  - *"Did you lose consciousness?"*
  - *"Did you lose control of your bladder or bowels?"*
  - *"Did you see spots or have changes in your vision?"*
  - These indicate near-fatal strangulation and should be documented for medical referral.

### After the Screen — Interpreting Results

#### Screens In as HIGH DANGER

The survivor screens in as high danger if:
- **Any of questions 1–4 are "yes"**, OR
- **3 or more of questions 5–11 are "yes"**, OR
- **The advocate's professional judgment indicates high danger** even if the numerical threshold is not met

**Immediate actions when a survivor screens high danger:**

1. **Name it directly but without panic:**
   > *"Based on what you've told me, your situation is very dangerous. Research shows
   > that when these factors are present, the risk of serious harm is high. I want to
   > make sure you have every possible protection available to you."*

2. **Connect to a DV hotline immediately.** If the survivor is willing, call together:
   - National DV Hotline: **1-800-799-7233**
   - Local DV program: _________________ (fill in for your region)

3. **Begin or update the safety plan.** Use `templates/safety-plan.md`. Prioritize:
   - Section 2 (during an explosive incident)
   - Section 3 (preparing to leave, if applicable)
   - Section 9 (go bag)

4. **Discuss protective orders.** If the survivor does not have one, explain the process and offer to accompany them to court. See Pod 4 (Legal Protection).

5. **Assess for strangulation.** If strangulation was reported, strongly encourage a medical evaluation — internal injuries from strangulation can be life-threatening even when no external injury is visible. Symptoms may appear 24–48 hours later.

6. **Document the screening result.** Use the `schemas/safety-assessment.json` schema with `immediateRisk.level` set to `"critical"` or `"high"`.

#### Does NOT Screen In as High Danger

Even if the survivor does not screen in as high danger:

1. **Do not dismiss the situation.** Say:
   > *"Your answers today suggest you may not be in the highest danger category right now,
   > but that does not mean you are safe. Any violence is dangerous, and situations can
   > change quickly. Let's talk about what you need."*

2. **Offer all standard services** — safety planning, legal advocacy, counseling, shelter information.

3. **Set a reassessment date.** Situations change. Screen again if:
   - The survivor reports a new incident
   - The survivor is planning to leave
   - 90 days have passed

4. **Document the screening result.** Use `immediateRisk.level` set to `"moderate"` or `"low"`.

---

## Strangulation — Special Protocol

Non-fatal strangulation is so strongly predictive of homicide that it warrants its own
section.

**Key facts for advocates:**

- A survivor who has been strangled by their partner is **750% more likely** to be killed by that partner (Glass et al., 2008)
- **50% of strangulation victims have NO visible injuries** — the absence of marks does NOT mean it did not happen
- **Delayed symptoms** can include difficulty swallowing, voice changes, neck pain, neurological symptoms, stroke, and death — even days later
- Many survivors minimize strangulation ("he just grabbed my neck," "he choked me a little")

**When strangulation is disclosed:**

1. **Validate immediately:**
   > *"What you're describing — being choked or having pressure put on your neck — is
   > extremely dangerous. Many people don't realize how serious this is, even if it
   > only lasted a few seconds."*

2. **Assess for symptoms now:**
   - Difficulty swallowing or breathing?
   - Voice changes (hoarseness, raspy voice)?
   - Neck pain or swelling?
   - Petechiae (tiny red dots) on face, eyes, or behind ears?
   - Dizziness, headache, or memory gaps?
   - Loss of consciousness during the incident?
   - Involuntary urination or defecation during the incident?

3. **Strongly recommend medical evaluation.** Internal injuries (laryngeal fracture, carotid artery damage, tracheal damage) can be life-threatening and are not visible externally.

4. **Document thoroughly.** Photograph the neck, face, and eyes (including behind ears) even if no visible injury is apparent. Note voice quality and any reported symptoms.

5. **Inform the survivor of the legal context.** In many states, strangulation is a felony offense regardless of visible injury. In Missouri, it is a Class D felony under RSMo § 565.073.

---

## Reassessment Schedule

| Trigger | Action |
|---------|--------|
| New incident of violence | Reassess immediately |
| Survivor planning to leave | Reassess immediately |
| Abuser released from jail/prison | Reassess immediately |
| Protective order granted, denied, or expired | Reassess within 48 hours |
| 90 days since last assessment | Routine reassessment |
| Significant change in abuser behavior | Reassess within 24 hours |
| Survivor reports new risk factors | Reassess within 24 hours |

---

## Documenting the Assessment

Use the `schemas/safety-assessment.json` schema. Key fields for lethality screening:

```json
{
  "assessorType": "dv-advocate",
  "situationType": ["intimate-partner-violence"],
  "immediateRisk": {
    "level": "high",
    "factors": [
      "strangulation-history",
      "abuser-threatened-to-kill",
      "violence-increasing-in-frequency-or-severity",
      "abuser-has-access-to-firearms",
      "survivor-plans-to-leave-or-recently-left"
    ],
    "assessorNotes": "Survivor screens in as high danger per LAP. Strangulation disclosed — referred for medical evaluation. Safety plan updated."
  },
  "consentToDocument": true
}
```

**Documentation best practices:**
- Record which screening tool was used and the date of your LAP training
- Note the survivor's demeanor and any disclosures made outside the formal screen
- If the survivor declines to answer a question, note "declined to answer" rather than leaving it blank
- If your professional judgment overrides the screen result (e.g., you assess high danger even though the numerical threshold was not met), document your reasoning

---

## Talking About Lethality — Language Guide

### What to say

- *"Research tells us that when these factors are present, the risk of very serious harm
  — including death — is real."*
- *"You know your situation best. How does what I'm saying match what your gut tells you?"*
- *"I'm not trying to scare you. I want you to have the full picture so you can make
  the best decisions for yourself."*
- *"Many survivors say they already knew the danger was high. This screen just confirms
  what you may already feel."*

### What NOT to say

- *"You're going to be killed"* — This disempowers and can cause the survivor to shut down
- *"You need to leave immediately"* — Leaving without a plan can increase danger; respect their autonomy
- *"Why haven't you left yet?"* — Never
- *"Your score is ___"* — Do not share a numerical score; discuss the factors and what they mean

---

## Integration with Other Tools

| Need | Tool | Reference |
|------|------|-----------|
| Build or update a safety plan | Safety Plan Builder | `templates/safety-plan.md` |
| Document the assessment in structured format | Safety Assessment Schema | `schemas/safety-assessment.json` |
| Document a specific incident | Incident Documentation | `templates/incident-log.md` |
| Find a local DV program for high-danger referral | Resource Directory | `templates/resource-directory.md` |
| Help with protective order filing | Legal Protection Pod | `references/legal-protection/pod.md` |
| Address tech-enabled surveillance or tracking | Digital Safety Pod | `references/digital-safety/pod.md` |
| Coordinate with law enforcement or other agencies | MDT Coordination | `templates/mdt-coordination.md` |

---

## Key Research References

- Campbell, J. C. (2003). Danger Assessment. Johns Hopkins University School of Nursing.
- Campbell, J. C., Webster, D. W., & Glass, N. (2009). The Danger Assessment: Validation of a lethality risk assessment instrument for intimate partner femicide. *Journal of Interpersonal Violence, 24*(4), 653–674.
- Glass, N., Laughon, K., Campbell, J., et al. (2008). Non-fatal strangulation is an important risk factor for homicide of women. *Journal of Emergency Medicine, 35*(3), 329–335.
- Maryland Network Against Domestic Violence. Lethality Assessment Program (LAP). mnadv.org.
- Messing, J. T., Campbell, J. C., Wilson, J. S., Brown, S., & Patchell, B. (2017). The Lethality Screen: The predictive validity of an intimate partner violence risk assessment for use by first responders. *Journal of Interpersonal Violence, 32*(2), 205–226.

---

*This guide is part of the Access to Safety project. It is intended for trained advocates
and is not a substitute for formal LAP training, the validated Danger Assessment instrument,
or clinical supervision.*
