# Electonic Health Record Systems
* What is the definiton of an EHR?
* How does an EHR differ from a paper record?
* What are the *functional* components of an EHR?
* What are the benefits of an EHR?
* What are the impediments to development and use of an EHR?
## 12.1 What is an EHR?
* patient record, patient's chart, medical record, health recovrd - all synonymous
### 12.1.1 Purpose of a Patient Record
* Reiser says:
  * recall Obs., inform others, instruct students, gain knowledge, monitor perf,  justify intervention
* Anticipate it'll hold longitudinal, whole life data of a person
* VA ensures it'll preserve data for at least 75 years
* **Electronic Health Record System** - tools used to manage info, the whole shabang
  * alerts, reminders, linkages, analysis, etc.
  * organize, interpret, and react
### 12.1.2 Ways in Which EHRs Differ from Paper
* At a small-scale, data can be represented in customized ways
  *  ie. date formats
* can include multimedia such as scalable radiology imaging or ECG video loops
* call attention to dangerous trends or outliers
* paper can only be accessed at one place at a time
* easier to stay HIPAA compliant
* care at the VA after Hurricane Katrina was a great example of paper vs EHR
* more legible
* pries for more data with leading questions
  * ex. smoker? -> how many packs per day -> how soon after waking?
* data fields are also a pain point
  * many fields are required, but may not be available at the time
* Metrics that EHRs are measured by to assess benefit
  * Comprehensiveness of information
    * does it cover data from everywhere and all kinds?
    * outpatient? inpatient? PCP? specialists?
  * Duration of use and retention of data
  * degree of structure of data
  * Ubiquity of access
* **hot fail over** - failure at one node doesn't mean failure everywhere
  * CLOUD! AND! SCALING!
## 12.2 Historical Perspective
* There were more EHRs prior to Lockheed-Martin's in El Camino Hospital, but this was the big one that spread to 200 hospitals
* CDS, linkages, and suggestions were first done by HELP at LDS, Columbia, CCC at Beth Israel, Regenstrief at Wishard, etc.
* Ambulatory care EHR adoption was slower than inpatient adoption
  * we're talking like in the 80s
## 12.3 Functional Components of an EHR
* What is considered a functional component?
### 12.3.1 Integrated View of Patient Data
* covering everything would be great, but not possible
  * some patient data is not electronic yet (old charts)
  * data from clinics/radiology sites/etc  might not be linked back to a centralized EHR and just sit on their own
  * aaaand lack of interop
* another difficulty is the lack of MPI
* ontologies are still an issue, but LOINC, ICD-10, CPT are helping
* HL7 is mentioned
### 12.3.2 Clinician Order Entry
* Super important because a big problem was transcription/communication errors at hand-off/transfer
* CDS gives pop-ups about allergies or conflicts in Rx
* can be simple as "take pill @ 5mg 3x" or an entire suite/regime
### 12.3.3 Clinical Decision Support
* Reminders and alert improve care process!!!
  * but oh god, pls don't be Practice Fusion and suggest pain management the way they did
* Can be done as batch jobs, iterating through subsets of a cohort in the EHR
  * provides notifications, emails, etc. to provider or patient
  * provider: double check/follow through, etc.; patient: schedule appointment, do test, etc.
  * batch jobs are the best way for patients who don't regularly visit
    * in contrast to "on-open" mode; since their record is never open
* but most often delivered at the CPOE phase
  * keep forgetting - CPOE is **COMPUTERIZED PHYSICIAN ORDER ENTRY**
  * useful because most alerts require an order to follow through
* can expedite an order with a single click
  * pre-populated forms based on patient record
  * oh god, opioids
  * best practice to annotate with rationale
* provide suggestions for once a lab is recorded or processed
  * or just alert a physician when it happens
* Reminders to outpatient settings quadrupled use of vaccines
* giving nurses alerts are useful for creating preventive measures
### 12.3.4 Access to Knowledge Sources
* an advanced/specialized CDS to provide linkages to NLIM PubMed/MedlinePlus and CDC info while documenting with a patient