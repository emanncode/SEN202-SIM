# SIM – Campus Security Questionnaire (Google Form Design)

**Title:** Campus Security & Crime Reporting Survey
**Description shown to respondents:**
"This survey is part of a SEN202 project to design SIM (Security Incident Mapping), a web platform that helps students, staff and landlords report security crimes on campus. Responses are anonymous. Please do not include your name or matric number. It takes about 5 minutes."

**Form settings to apply in Google Forms**
- Collect email addresses: **Off** (keeps responses anonymous)
- Limit to 1 response: **Off**
- Shuffle question order: **Off**
- Progress bar: **On**
- Confirmation message: "Thank you. Your response has been recorded."

---

## Section 1 – Consent and Respondent Profile

**Q1. Do you agree to take part in this survey?** *(Required, Multiple choice)*
- Yes, I agree and am 18 or older
- No, I do not agree *(go to section based on answer → Submit form)*

**Q2. Which best describes you?** *(Required, Multiple choice)*
- Student
- Staff (academic or non-academic)
- Landlord / property owner
- Other community member
- Prefer not to say

**Q3. Where do you live or work on or near campus?** *(Required, Dropdown)*
- On-campus hostel
- Off-campus hostel / student villa
- Staff quarters
- Rented apartment (own accommodation)
- Office / lecture area only (no residence nearby)
- Other

**Q4. What is your age group?** *(Required, Multiple choice)*
- Under 18
- 18–24
- 25–34
- 35–44
- 45 and above

---

## Section 2 – Experience of Security Crimes

**Q5. In the last 12 months, have you witnessed or personally experienced a security crime on or near campus?** *(Required, Multiple choice)*
- Yes, I experienced it
- Yes, I witnessed it
- Yes, both
- No *(go to section based on answer → Section 4)*

**Q6. What type(s) of crime did you experience or witness?** *(Required, Checkboxes)*
- Stabbing / physical assault
- Rape or sexual assault
- Theft / stealing
- Armed robbery
- Murder / attempted murder
- Kidnapping
- Vandalism
- Cultism-related violence
- Other (please specify) *(Short answer)*

**Q7. Where did the incident(s) happen?** *(Required, Checkboxes)*
- Inside a hostel or villa
- Hostel or villa compound gate
- Lecture theatre / classroom
- Library
- Roads or footpaths on campus
- Bush paths or unlit areas
- Market or shops near campus
- Other (please specify) *(Short answer)*

**Q8. At what time of day did it happen?** *(Required, Multiple choice)*
- Morning (6am – 12pm)
- Afternoon (12pm – 6pm)
- Evening (6pm – 10pm)
- Night (10pm – 6am)
- I don't know

**Q9. How severe was the most recent incident in your view?** *(Required, Linear scale 1–5)*
- 1 = Minor, 5 = Very severe

---

## Section 3 – Reporting Behaviour

**Q10. Did you report the incident to anyone?** *(Required, Multiple choice)*
- Yes, to campus security
- Yes, to the police
- Yes, to my landlord or hostel management
- Yes, to a friend or family member only
- No, I did not report it
- Not applicable (no incident)

**Q11. If you did NOT report, why not?** *(Show only if Q10 = "No, I did not report it", Checkboxes)*
- I did not know where or how to report
- I was afraid of retaliation
- I did not think anything would be done
- The process is too slow or stressful
- I did not trust the authorities
- I did not want to be identified
- It was not serious enough
- Other (please specify) *(Short answer)*

**Q12. Which of these would make you more likely to report a crime?** *(Required, Checkboxes, choose up to 3)*
- Anonymous reporting
- Reporting from my phone in under 2 minutes
- Seeing the status of my report
- Being able to attach a photo or video
- A map showing crime hotspots
- A quick emergency button
- Faster response from security

---

## Section 4 – Perception of the SIM Platform

**Q13. How likely are you to use an online platform like SIM to report a campus security crime?** *(Required, Linear scale 1–5)*
- 1 = Very unlikely, 5 = Very likely

**Q14. Which feature do you think is most important?** *(Required, Multiple choice)*
- Anonymous submission
- Location pin on a map
- Photo or video upload
- Live crime map
- Report tracking
- Emergency contact button

**Q15. How would you prefer to access SIM?** *(Required, Multiple choice)*
- Mobile browser
- Desktop or laptop browser
- SMS / USSD
- Both mobile and desktop
- I would not use it

**Q16. What concerns do you have about reporting crime online?** *(Optional, Paragraph; remind respondents not to include names or identifying details)*

---

## Section 5 – Staff and Landlord Questions

*Show this section only if Q2 = Staff or Landlord. Otherwise go to Section 6.*

**Q17. Do you know how to contact campus security quickly?** *(Required, Multiple choice)*
- Yes, I have the direct contact
- I know the general number only
- No

**Q18. What security measures are present at your premises or workplace?** *(Required, Checkboxes)*
- CCTV cameras
- Security guard or gateman
- Working gate locks
- Street or compound lighting
- Fence or perimeter wall
- Alarm system
- None of these

**Q19. Do you screen or register tenants or residents?** *(Show for Landlord only, Required, Multiple choice)*
- Yes, with ID and references
- Yes, with ID only
- No

**Q20. Would you be willing to report incidents on your premises through SIM?** *(Required, Multiple choice)*
- Yes
- Maybe, if it is anonymous
- No

---

## Section 6 – Suggestions

**Q21. In your opinion, what is the single most effective step to reduce crime on campus?** *(Optional, Paragraph)*

**Q22. Would you like to be contacted about the SIM project?** *(Optional, Short answer: email address)*

---

## Section 7 – Safety Perception and Trust

**Q23. How safe do you generally feel moving around campus and nearby student residential areas?** *(Required, Linear scale 1–5)*
- 1 = Very unsafe, 5 = Very safe

**Q24. What would make reporting a security concern feel safer or more trustworthy?** *(Optional, Paragraph; remind respondents not to include names or identifying details)*

---

## Analysis Plan (what each question feeds)

| Question(s) | Purpose | Feeds into |
|---|---|---|
| Q2, Q3 | Identify user groups | SRS user classes |
| Q5–Q9 | Size and type of the problem | Ishikawa problem statement |
| Q10–Q11 | Underreporting causes | Ishikawa "People / Process" bones, SRS anonymity requirement |
| Q12, Q14 | Priority features | SRS functional requirements |
| Q13, Q15 | Adoption and access channel | SRS non-functional requirements (usability, responsiveness) |
| Q16, Q21 | Trust and privacy concerns | SRS security and privacy requirements |
| Q17–Q20 | Landlord and staff role | Use case actors and use cases |
| Q23 | Perceived campus safety | SRS background and Ishikawa environment causes |
| Q24 | Conditions for trusted reporting | SRS privacy and ethical handling requirements |

---

## Sample Responses (illustrative only)

> **Important:** These are example answers written to show what a completed form might look like. They are **not real survey data**. Replace them with real responses before submitting, or clearly label them as illustrative in your report.

| Resp. | Q2 | Q3 | Q5 | Q6 | Q7 | Q8 | Q9 | Q10 | Q11 | Q12 | Q13 | Q15 | Q18 |
|---|---|---|---|---|---|---|---|---|---|---|---|---|---|
| 1 | Student | Off-campus villa | Experienced | Theft | Roads or footpaths | Night | 3 | Did not report | Afraid of retaliation | Anonymous, faster response | 4 | Mobile | – |
| 2 | Student | On-campus hostel | Witnessed | Stabbing | Bush paths | Night | 5 | Campus security | – | Map, faster response | 5 | Both | – |
| 3 | Staff | Staff quarters | No | – | – | – | – | – | – | Anonymous | 3 | Desktop | CCTV, gate lock |
| 4 | Landlord | Rented apartment | Both | Theft, vandalism | Compound gate | Night | 4 | Landlord | – | Photo upload | 4 | Both | Gate lock, fence |
| 5 | Student | Off-campus villa | Experienced | Armed robbery | Market or shops | Evening | 4 | Did not report | Did not know where to report | Emergency button | 5 | Mobile | – |

**Summary of illustrative results**
- Most reported crime types: theft and stabbing or physical assault.
- Most common locations: unlit bush paths, roads, and compound gates, mostly at night.
- Main reason for not reporting: fear of retaliation and not knowing where to report.
- Most requested features: anonymous reporting and faster response.
