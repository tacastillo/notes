# Chapter 17 - Consumer Health Informatics and Personal Health Records
## Objectives
- [ ] Define the central tenet of consumer health informatics
- [ ] Define and explain the issues that biomedical informatics research can address relating to:
  - [ ] Consumer communication
  - [ ] Decision-making
  - [ ] Information access needs
- [ ] Issues that technology are trying to address will be still be prevalent in the future. Describe the larger bioinformatics topics this technology is being used to address.
- [ ] Define:
  - [ ] Patient portals
  - [ ] Personal health records
  - [ ] Patient-controlled health records
  - [ ] Personal health applications
## 17.1 - Introduction
* side bar: **etiological** - (in medicine) causing or contributing to the development/growth of a disease or condition
* *complexity* and *collaboration* define how healthcare in the 21st century
  * complexity arises from a deeper understanding of health and disease
  * collaboration is more than just between clinician to clinician
    * also about how the patient, family, community, population and society contribute to health/well-being
* Four common HC challenges that consumer informatics specifically address:
  * consumer engagement, information sharing, communication and decision facilitation
### 17.1.1 - The Challenge of Improving Consumer Engagement
* forms of patient participation: shared decision-making, self-care and collaborative practices
* **Distributed-managed care models** - consumers are their own case workers and they have agency to pick and choose their providers
* Central tenet is that not even though not all patients will participate, those that do will lead to higher quality care than patients than don't
  * Extrinsic motivators (lol Rally, money, goods, praise) can help woo patients that aren't naturally inclined to be involved in their own care
### 17.1.2 - The Challenge of Improving the Information Available to Consumers
* Old and suboptimal ways to educate/convey new findings to the public: pamphlets, (newspaper) articles, phone calls
* KPIs to look for when picking a modality: health literacy, widespread access, appropriately timed/placed, reaching all possible audiences
### 17.1.3 - The Challenge of Improving the Communication Among Consumers and Providers
* Consumer-provider interactions
  * CHI (Consumer Health Informatics) primes patients to be able to have educated/productive discussions with their providers
* Consumer-to-consumer communication has always been difficult
  * social media (Vytality Health)
  * historically: support groups for diseases run by churches, community centers, or health institutes
### 17.1.4 - The Challenge of Improving Consumer Decision-Making
* Collecting data isn't the most important part of this process
* The importance is consumers making educated, high-quality and *actionable* decisions and act on them
* People used to rely on libraries, conversations, word-of-mouth
  * No attention to the actual evidence, risks/benefits and their personal differences
  * We really haven't moved any further with WebMD, folks
## 17.2 - Historical Perspective on Consumer Health Informatics
### 17.2.1 - The Rise of Consumer-Oriented Health Communications
* goal: move patients from being passive recipients to actively involved
  * factor in a patient's values, preferences and lifestyle
* US Federal Children's Bureau
  * Mothers would send paper letters to them asking questions
* Primarily through mail, then television shows, videos, etc.
  * "consumer health broadcasts"
  * The OG Dr. Oz 🙄
  * Daytime television and radio shows
* Since the 1940s, hospitals had computerized forms filled out by patients to calculate risk
### 17.2.2 - Early Advances in Consumer Information Sharing and Decision Making
* Self-help and self-monitoring movement
* Focused on education and giving short lists of therapies/treatments to pick from... kinda
* BARN (think DARE, but with games)
  * wow that's a lot of school assemblies
* Internet was also used to educate
  * Games took time to build, but had the best adoption rate
### 17.2.3 - Early Advances in Consumer-Consumer Interaction
* Online coping/support groups having reduced feelings of anxiety/hopelessness and improved coping skills and life expectancy
* The increased used of the internet for consumer education/decisions also comes with a decrease in general quality in health information on the internet
  * No source of moderation/filtering/quality checks; fake news
### 17.2.4 - Early Advances in Consumer Decision-Facilitation
* In the 1970s, there was a move towards more interactive and personalized content
* "just-in-time"
## 17.3 - Current Trends
### 17.3.1 - Consumer-Facing Software
* > "The home and community are fast becoming the most common sites where health care is provided."

| Mode of Engagement | Definition | Examples | 
| ----------- | ----------- | ----------- |
| Communication | Patient-patient, computer-patient, patient-provider | Patient portals, Patient-physician emails, online support groups, social networks |
| Data Storage | Patient-centered data repos for patient-entered/-reported data | PHRs, data portals |
| Behavior Management | Tools to support personal health goals, via data storage, info sharing, and communication | Weight management tools, apps, trackers, medication reminder apps |
| Decision Aids | Enable people to weight benefits, harms, evidence and scientific uncertainty when making decisions | Calculators |
### 17.3.2 - Communication
#### 17.3.2.1 - Patient-Centered Communication
* Not uncommon for patients to see up to seven different providers for a chronic condition
* IOM (Institute of Medicine) defines 10 rules to improve health care quality
  * 6 of those 10 rules involve patient engagement.
* NHII (National Health Information Institute)
* **data liquidity** - the property of data being able to be interoperable or movable across systems/software, unlike conventional EHR data
  * > Facilitated by patients being able to direct and access other's access to their information according to laws and protocols
  * OTC meds, home therapy for allergies/trauma, physiologic monitoring (ECGs, continuous monitors, etc.)
#### 17.3.2.2 Electronic Support Groups
* ISG (Internet Support Group)
* 28% of internet users have visited at least one ISG
* Four primary modes of communication
  * Email lists, instant messaging, bulleting boards and chat rooms
  * Slow increase group videoconferencing and socialization interventions
#### 17.3.2.3 Social Networks
* "Patients Like Me"
* Consumers on sites like these are highly willing to contribute data and observations without compensation to accelerate learning about their disease
* Social networks short circuits the traditional research enterprise
  * Rewards participants and researchers
### 17.3.3 - Patient Access to Health Information
* **Guardian Angel Proposal** - [Website](www.ga.org) - vision of a web that manages a patient's health records, decision support, insurance benefits, education and communication
#### 17.3.3.1 Portals
* **Portals** - Consumer-facing systems attached to EHRs that allow patients to view clinical or claim data
  * ex. Epic's MyChart
* Additional Functionality
  * patient-physician messaging, appointment scheduling, viewing/managing bills
#### 17.3.3.2 Personal Health Records
* **PHR (Personal Health Records)** - an application that patients can manage, access, and share their own health information with others in a private and secure environment
* Paper version: immunization record books
* 1:1 mapping vs EHR's many:many mapping
* Enabled by a patient's right to their data from the institutions they receive care from
  * Justified via HHS' **Meaningful Use**
#### 17.3.3.3 Personally-Controlled Health Records
* **PCHR - Personally-controlled health records** - a special form of PHR... undefined ☹
  * But basically Mint or Quicken for health data
  * Roll up the data from all your healthcare institutions
* *Indivo* - super example of PCHR architecture, started off at Harvard as PING (Personal Internetworked Notary and Guardian)
* Pulling from EHRs is difficult because EHRs are resistant to interoperability
* Allow patients to selectively authorize access to family, hospitals, specific providers, researchers, proxies, etc.
### 17.3.4 Behavior Management
* health prevention through wellness activities
  * active lifestyle development, stress reduction, smoking cessation, weight control
  * self-care
  * *preventative medicine*
* Apps a great medium for this
| Name and source | Summary |
| --- | --- |
| Self-efficacy | an individual's impression of their own ability to perform a task, either physically or mentally |
| Social cognitive therapy | behavior change is dependent on personal, environmental and behavioral elements; interdependent elements |
| Theory of planned behavior | link between attitudes and behavior; behaviors viewed positively and supported by others are morely likely to happen |
| Transtheoretical/stages of change | 5-stages process; fluid stages |
### 17.3.5 Consumer Decision-Making
* Informing users
* Building question-driven decision trees
* Calculators
* Descriptions and testimonials about future outcomes are shown to increase consumers' knowledge and satisfaction with treatment decisions
* Still a challenge to integrate into a clinical workflow
### 17.3.6 Consumer Information Access
* EHRs aren't designed to give data "just-in-time" but rather "just in case"
#### 17.3.6.1 Passive Information Access
* ...stuff you can read; or presentations
#### 17.3.6.2 Active Information Access
* Voice assistants
* Automated feedback
* Alerts
* Dashboards
* Text messaging
* Reminders
  * ex. appointment reminders reduce no-show rates
## 17.4 Opportunities and Challenges
