# Customization Guide — Fork and Adapt Access to Safety

This guide walks you through forking the Access to Safety project and adapting it for a
new region, language, or community context. You do not need to be a developer to do most
of this work. The main tasks are research, writing, and careful verification.

---

## Who This Guide Is For

- Domestic violence advocates who want a resource directory for their region
- Volunteers who want to create a localized version of this project
- Developers building on this framework for a specific community
- Organizations that want to white-label or adapt this system

---

## Prerequisites

### Required
- A GitHub account (free at github.com)
- Basic ability to edit text files (Markdown is just formatted plain text)
- Access to a phone and internet to verify resources

### Helpful but Not Required
- Familiarity with Markdown formatting
- Knowledge of the local DV services landscape
- A local DV advocate or organization as a partner/reviewer

### Time Estimate
- Forking and basic setup: 30–60 minutes
- Populating one resource pod fully: 2–4 hours
- Full directory for a mid-sized city: 10–20 hours of research and verification
- Ongoing maintenance: 2–4 hours per quarter

---

## Step 1 — Fork the Repository

1. Go to the Access to Safety repository on GitHub.
2. In the upper right corner, click **Fork**.
3. Choose your personal account or an organization account as the destination.
4. Give your fork a descriptive name, such as `access-to-safety-chicago` or
   `access-to-safety-travis-county`.
5. Click **Create fork**.

You now have your own copy of the project. Changes you make will not affect the original
repository unless you choose to submit them back (see Step 8).

---

## Step 2 — Clone Your Fork Locally (Optional, for Larger Edits)

If you are comfortable with the command line:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-FORK-NAME.git
cd YOUR-FORK-NAME
```

If you prefer to edit in the browser, you can edit files directly on GitHub by clicking
the pencil icon on any file. For adding many resources, a local editor like VS Code is
more efficient.

---

## Step 3 — Update the README

Open `README.md` and update:

- **Region name** — Replace references to the generic project with your specific region.
- **Maintainer contact** — Add a way for users and contributors to reach you.
- **Coverage disclaimer** — Note which geographic area this fork covers and what it does not cover.
- **Last updated date** — Set this to today; update it whenever you do a review.

Do not remove the attribution to the original Access to Safety project. Add your
attribution alongside it.

---

## Step 4 — Populate the Resource Directory

Open `templates/resource-directory.md`. This is your primary work file.

### 4a. Fill in the Directory Metadata block at the top

```
Region covered: [Your city, county, or region]
State / Province: [Your state]
Last full review date: [Today's date]
Reviewed by: [Your name or organization]
```

### 4b. Work through the pods one at a time

Start with Pod 1 (Crisis & Emergency Safety) — these resources are the most urgently needed
and should be verified first. Then work through the remaining pods.

**For each resource you add:**

1. Find the organization (see Step 5 for how to find resources).
2. Call them directly to verify: phone number, address, hours, services, eligibility, cost.
3. Visit their website to confirm and supplement.
4. Fill in every table column you were able to verify. Leave cells blank if unknown.
5. Record the date you verified and your name (or "volunteer") in the last two columns.

### 4c. Add the state-specific legal section in Pod 2

This is one of the most valuable things you can customize. Research and fill in:

- Types of protective/restraining orders available in your state
- How to apply (self-represented vs. attorney required)
- Emergency order process (same-day, after-hours availability)
- Filing fee and fee waiver process
- Relevant statutes by name and number

See Step 6 for how to research state laws.

---

## Step 5 — How to Find Local Resources

### Starting Points

| Source | What You'll Find |
|---|---|
| **211.org** or dial 2-1-1 | Broad social services database, searchable by zip code |
| **thehotline.org/get-help/domestic-violence-local-resources/** | DV-specific local resources |
| **domesticshelters.org** | Shelter locator with detailed program info |
| **womenslaw.org/find-help/advocates-and-shelters** | State-by-state advocates list |
| **rainn.org/get-help/local-counseling-centers** | Sexual assault resources by zip |
| **aardvarc.org** | State coalitions and member organizations |
| **State DV coalition website** | Your state's coalition maintains member directories |
| **2-1-1 database** | Many states have a searchable 211 database online |
| **Google / local news** | Search "[city] domestic violence shelter" or "DV resources [city]" |

### How to Find Your State Coalition

Search: `[state name] coalition against domestic violence`

State coalitions typically maintain member directories and can refer you to local programs.
They may also be able to review your resource list for accuracy.

### How to Verify a Resource

Call the organization and say something like:

> "Hi, I'm compiling a resource directory for survivors of domestic violence in [region].
> I want to make sure our listing for your organization is accurate. Can you confirm your
> phone number, address, hours of operation, and main services? And are there any eligibility
> requirements or costs survivors should know about?"

Note the name of the person you spoke with and the date.

---

## Step 6 — How to Look Up State-Specific Laws

### Protective Order Laws

- **WomensLaw.org** — Plain-language summaries of each state's protective order laws,
  organized by state. Start here: womenslaw.org/laws
- **ABA Commission on DV** — Legal resources and state law summaries
- **State legislature website** — For the actual statute text (search "[state] legislature
  code" or "[state] statutes online")

### What to Document for Each State

When researching protective orders for your state, find and record:

1. Names of each order type (e.g., "Emergency Protective Order," "Final Restraining Order")
2. Who can file (victim, police, other)
3. Where to file (courthouse, police station, online)
4. Cost and fee waiver availability
5. Duration and renewal process
6. What behaviors can be prohibited
7. Enforcement mechanism (criminal penalty, contempt)
8. Any specific provisions for DV vs. stalking vs. sexual assault

### Immigration-Related Laws

If your region has a significant immigrant population, also document:
- VAWA self-petition (federal)
- U visa and T visa eligibility
- Local policies on immigration enforcement at courthouses and shelters
- Local legal organizations that handle immigration + DV cases

---

## Step 7 — What to Change in Each File

| File | What to customize |
|---|---|
| `README.md` | Region name, maintainer contact, coverage area, last updated |
| `templates/resource-directory.md` | All resource tables, directory metadata, state law section |
| `templates/safety-plan.md` | Local hotline numbers, any region-specific safety considerations |
| `templates/incident-log.md` | Local court information, any jurisdiction-specific legal notes |
| `schemas/resource-entry.json` | Only if you need to add region-specific fields |
| `references/` | Add local legal references, state statute links |

### Files You Should NOT Change Without Good Reason

- The core structure of the safety plan template — it is based on evidence-based safety
  planning frameworks
- The incident log template — it is designed for legal admissibility
- JSON schema files — changing these will break compatibility with other tools

---

## Step 8 — Testing Your Customization

Before sharing your fork with anyone:

### Accuracy Check
- [ ] Every phone number in the directory has been called and answered (or you have
      noted it is unverified)
- [ ] Every address is confirmed (not just copied from an old source)
- [ ] Hours are current — organizations frequently change hours without updating websites
- [ ] Eligibility and cost information is accurate and complete

### Completeness Check
- [ ] Pod 1 (Crisis & Emergency) is fully populated — this is the minimum viable directory
- [ ] At least one shelter option is listed
- [ ] At least one legal aid option is listed
- [ ] National hotlines are included as fallback options
- [ ] Directory metadata is filled in (region, date, reviewer)

### Readability Check
- [ ] A non-technical person can navigate the directory easily
- [ ] Tables render correctly (preview in GitHub or a Markdown viewer)
- [ ] Language is plain, direct, and accessible
- [ ] No jargon without explanation

### Safety Check
- [ ] No personal information about survivors or volunteers is included in the public files
- [ ] Contact information listed is for organizations, not individuals (unless they have
      consented to be listed publicly)

---

## Step 9 — Submitting Back to the Community

If your fork adds value that could help other regions — for example, you have created a
reusable framework for a particular state's laws, or added new template sections — consider
contributing it back to the original project.

### How to Submit a Pull Request

1. Make sure your fork is up to date with the original repository:
   ```bash
   git remote add upstream https://github.com/ORIGINAL-OWNER/access-to-safety.git
   git fetch upstream
   git merge upstream/main
   ```

2. Push your changes to your fork on GitHub.

3. On GitHub, go to your fork and click **Contribute > Open pull request**.

4. Write a clear description of what you added or changed and why it is useful to other
   regions or users.

5. The project maintainers will review and may ask questions or request changes.

### What Makes a Good Contribution

- A new template section that addresses a need not currently covered
- Improvements to the AI instruction blocks that make responses safer or more helpful
- A schema improvement that adds useful fields
- A framework for a state's laws that others can adapt
- Bug fixes (broken links, incorrect information in the default templates)

### What to Keep in Your Fork Only

- Your region's specific resource data (this is only useful locally)
- Personal customizations for a specific organization's workflow
- Anything that contains personal information

---

## Step 10 — Maintaining Your Fork

A resource directory that is not maintained becomes harmful — it sends survivors to
organizations that no longer exist or have changed their services. Commit to a maintenance
schedule before you publish.

### Recommended Maintenance Schedule

| Task | Frequency |
|---|---|
| Check all phone numbers | Every 6 months |
| Review hours and services | Every 6 months |
| Check for new organizations to add | Annually or when you hear of one |
| Review state law sections for changes | Annually |
| Update "Last Verified" dates | Every time you verify |
| Check for updates to the upstream project | Every 3 months |

### How to Pull Updates from Upstream

```bash
git fetch upstream
git checkout main
git merge upstream/main
```

Review the changes carefully before merging — updates to templates may conflict with
your local customizations. Resolve conflicts by keeping what is most accurate for your
region while incorporating improvements from the upstream project.

### Handing Off to a New Maintainer

If you can no longer maintain your fork:

1. Find a successor — a local DV organization, an advocate, or a volunteer
2. Add them as a collaborator on your GitHub fork (Settings > Collaborators)
3. Document the maintenance procedures and your local contacts for verification
4. Update the README with the new maintainer's contact information
5. Post a note to the project community that you are transferring maintenance

Do not simply abandon a published directory. Archive it or mark it clearly as unmaintained
so users know not to rely on it.

---

## Getting Help

- **Project discussions:** Open an issue on the main Access to Safety GitHub repository
- **DV sector knowledge:** Contact your state DV coalition
- **Technical help:** The GitHub documentation at docs.github.com covers forking, pull
  requests, and Markdown in detail
- **Legal research help:** WomensLaw.org and your state's legal aid program can help
  review the accuracy of your legal resources section

---

*This guide is part of the Access to Safety project. Thank you for the work you are doing
to make safety resources more accessible in your community.*
