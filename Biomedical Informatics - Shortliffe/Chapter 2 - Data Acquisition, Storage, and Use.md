# Chapter 2: Biomedical Data, Their Acquisition, Storage, and Use 
## Who Collects Data
* Clinicians
	* Can collect data via conversing/observing patients + instrumentation
	* Not just a primary source of the actual recording
		* Also dictates what data is to be recorded next
			* Requests labs, tests, diagnostics, surgeries, imaging, etc.
	* Scribes are cool, but add an intermediary layer between physician and documentation source (EHR)
* Nurses
	* HCPs that receive the most actual face time and interaction with patients
	* observation, history taking, and examination
	* Builds the strongest relationships with patients
  	* opens opportunity for more "honest" patient records and psycho-social observations
*  Other HCPs
  * office/admin staff - demographic, claims, and  financial information
  * Physical/respiratory/occupational therapists - progress, treatments, suggestions
  * Lab personnel - tests
  * Radiology techs - imaging
* Pharmacists - medications, usage, adherence, drug allergies
* Instruments
  * lab machines, imaging, *monitoring*
  * Can export single data points (thermometers), continuous streams (ECGs, CGMonitors) or images (pictures, imaging, etc.)
## Uses of Health Data
* EHRs suck, but they're still somehow better than paper records
  * Theoretically
  * Longitudinal access across an institution would be great; even better across institutions
  * Creates the Basis of a Historical Record
  * record of what health conditions and observations *have* been made
  * allows the care team to look at trends over time
  * history and reoccurence of symptoms/illnesses
  * medications, interventions, decisions, **and reasoning behind them**
  	* hopefully lots of metadata behind each
  * *Allows for the use of population-level insights*
  	* statistical models, similarities, comparisons, analyses
* Support communication among providers
  * historically, a patient only had one doctor from youth to adulthood and saw them for everything
  	* Specialization changed that and fragmented patient-doctor relationships and continuous history
  * Recording patient data leaves a trail and medium for multiple doctors to communicate with each other about a patient through the documentation, patient history and clinical notes
  * Emphasis on the importance of **continuity of care**
* Anticipate future health problems
  * Can use the history to predict/diagnose/create a prognosis of the future
* assists in screening risk factors
  * longitudinal view allows for ease of prescribing interventions (diet/lifestyle changes)
* Record standard preventative measures
  * ie. vaccinations, smoke cessation, safe sex practices, interventions such as dietary changes
* Identify deviations from expected trends
* Provide a legal record
  * safety for life/medical insurances
  * Malpractice coverage
  * other legal actions
* Support clinical research
  * Clinical Trials!
	* Looking at multiple patients' data!
* aggregation, statistics, analyses once again
  * **Retrospective studies** - the good shit
	* Using historical data sets to do research
	* Common in epidemiology
	* Calculating risks of smoking, lung cancer, finding proportions, heart disease, death rates, recidivism/recurrence, etc.
## Weaknesses of traditional medical record system (as in paper charts; ~holy crap how old was the first edition of this book~)
* Recording data aint worth shit if you can't find it later
  * Metrics of "finding" data: resolution (actually finding it), speed, legibility/interpretablity, reliability
    * Patient records (especially those with chronic conditions) can be large and cumbersome to sift through
  * Metrics also apply to being able to *update* this data
* Redundancy and Inefficency
  * If you're seeing multiple physicians, you're going to get redundant clinical notes and observations
    * Often there's some sort of collision
    * Some clinicians prefer a certain type of shorthand, whereas other prefer another; labeling and categorizing can vary too.
  * For imaging, the time it takes to get a scan inserted into an EHR may take a couple days due to personnel and logistics, so the radiologist has to put in notes manually to cover for the gap between them actually seeing the scan and when the scan is actually accessible by other physicians
* Influence on clinical research
  * it was hard to do population-level clinical research back in the days of paper records
  * **retrospective studies** vs **prospective studies**
    * retrospective looks into a question that was not the focus of a previous study
    * prospective is conventional scientific method: create a hypothesis, run experiment+collect data
  * studies try to be as random and double-blind as possible
  * Finding the right datum after you get a record
    * Arduous and painful as hell, even if you're using an EHR
    * ex. find a drug that an admitted patient was taking
      * ok, you can look at prescription, but did they actually take it?
      * ok, now you cross-check with drug administration, but was there an issue with them taking it?
      * ok, now check nurse notes
        * but which nurse: nurse at admission? bedside nurse? surgical nurse?
  * Passive nature of paper records
    * paper records can be omitted/forgotten/ignored at the level of the entire form or just a field
    * electronic records are active and dynamic
      * active - can have required fields/required forms
        * can have automated quality control
        * can provide more detailed feedback at the patient- or population- level
      * dynamic - different forms can be suggested based on purpose and intent and context
        * Can also generate warnings or advice based on inputs
          * ex. prescribe a drug and get a modal saying the patient is allergic to it
## New Kinds of Data and the Resulting Challenges
* Human Genome Project!!
  * created so many possibilities that the possibilities became problems
  * how do you use and store all of this?!
  * **personalized medicine** - the extra good shit
    * the integration of clinical diagnostics and genomics
    * using a patient's genes to deduce the best care plan and course of action
## The Structure of Clinical Data
* Physicists, math, chemistry and other scientific disciplines have conventions and consistent vocabulary
* Medicine has lacked creating such an ontology or __nomenclature__
  * there have been parties that have brushed it off as "medicine is an art, not a hard science"
    * EHRs and data storage have put a huge wrench in that
  * ie. what is an "upper respiratory infection"?
    * Are we talking the trachea or are we talking on the main stem bronchi?
	* ie. how large is large enough for "cardiomegaly" (abnormally large heart)
	* shortness of breath vs. dyspnea
  	* programs and SQL queries can't decide whether they're the same or not
	* sooo much imprecision
### Coding Systems
* WOOHOOO
* an attempt at creating an ontology of conditions, drugs, observations, etc.
* Health reporting requirements
  * ie. having to report gonorrhead, syphilis or TB to the CDC's local branches
  * having a coding system and concrete definitions make these much easier
  * ICD
    * WHO invented ICD (**International** Classification of Disease)
      * Fun fact: Before ICD10, US was actually using ICD9-CM (*Clinical Modifications*)
    * derived from a terminology primarily used for epidemiological use, but surprise! It's what EHRs prioritize!
      * you can still feel that it originated for those purposes though
        * 500 different codes for describing tuberculosis
  * SNOMED-CT
    * Pathologists and other lab-oriented HCPs made SNOP (Systemized Nomenclature of Pathology)
      * Evolved into everyone's favorite _SNOMED_ (Systemized Nomenclature of Medicine)
    * It's actually called __SNOMED-CT__ because it merged with Great Britain's *Read Clinical Terminology*
    * Managed by the International Health Terminology Standards Development Organization in Copenhagen
    * Historical nuances
      * lots of exquisite detail on pathological findings, recently started adding patient functional status dimensions
        * often too coarse (not detailed enough in granularity) for use at bedside by a nurse, but super useful for a hematologist!
  * CPT
    * Current Procedural Terminology
    * developed by AMA (American Medical Association)
    * Motivations
      * Pooling/aggregation of patient data (suprisingly!)
      * Charging/billing/insurance (what it's really used for)
    * 
  * some practitioners often roll up and use the higher-level terminology if a coding system has too much fine detail and variety in codes
## The Data-to-Knowledge Spectrum
* **datum** - a single observational point that characterizes a relationship
  * or a value of a specific parameter for a specific object
    * "object" is a flexible term in terms of hierarchy
      * an object can be a blood pressure level, or a whole patient
  * not necessarily an observation
  * **information** - analyzed data that have been suitably curated and organized so that they have meaning
    * data that has been given *meaning*
  * **knowledge** - derived through analysis of information that was in turn derived from data.
  * **heuristic** - a process/methodology/way of thinking derived from knowledge
  * Example of the hierarchy - 
    * datum - patient has a blood pressure of 180/110
      * parameter is blood pressure
      * object is patient
      * value is 180/110
    * information - patients with high blood pressure are more likely to have heart attacks
    * knowledge - reduce your blood pressure, mi dood
      * how? reducing salt content in foods
      * additional nuances:
        * not helpful for patients that're of socioeconomic disadvantage because they are less likely to have access to low sodium food
  * **database** - collection of individual observations without any summarizing analysis
    * aka, probs doesn't have any metadata with it
    * pool/aggregate the data across an EHR and you that's when you develop *information*
  * **knowledge base** - collection of facts, info, heuristics and models that can be used for analysis or deriving additional information
    * building a knowledge base that can link data semantically through knowledge can be interpreted as CDS
      * knowledge-based systems; huh, who woulda guessed