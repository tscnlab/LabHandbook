# Variables

## Scope

The following presents a standardised way for naming variables and their response options, specifically arising from questionnaires and surveys.

## Definition

We agreed to use the following conventions for demographic variables and answer possibilities and for specific meaaurement instruments as for the Karolinska Sleepiness Scale (KSS) (10 is optional).

The standard YesNo question is a binary question with 1=Yes and 0=No.
If more answer options are needed, the question must be named other, for example YesNomO (for YesNo multiple otions).

The option "Prefer not to say" is always the last option in single choice answers.
The option "Not collected" is not provided as a choice to select, this is an internal coding.
* For "Preferred language" the following note has to be added to the question:
"Note: If you do not prefer either of the languages, you are not eligible for the study.
       This means you can not participate in the study."


### Standard Demographic Variables


| Description        | Variable           | Meaning                                  | Code | Question              | Notes           | Meaning German | Question German |
|--------------------|--------------------|------------------------------------------|------|-----------------------|-----------------|----------------|-----------------|
| YesNo              | yesno              | Yes                                      | 1    |                       | binary question |   Ja           |                 |
|                    | yesno              | No                                       | 0    |                       |                 |   Nein         |                 |
|  |  |  |  |  |  |  |  |
| Sex                | sex                | Female                                   | 1    | Sex assigned at birth |                 |  Weiblich      | Bei der Geburt zugewiesenes Geschlecht |
|                    | sex                | Male                                     | 2    |                       |                 |  Männlich      |                  |
|                    | sex                | Intersex                                 | 3    |                       |                 |  Intersexuell  |  |
|                    | sex                | Not collected                            | -1   |                       |                 |  Nicht erhoben |  |
|                    | sex                | Prefer not to say                        | 0    |                       |                 |  Ich möchte keine Angaben dazu machen  |  |
|  |  |  |  |  |  |  |  |
| Gender             | gender             | Woman                                    | 1    | What gender do you identify with?|                 |  Frau | Mit welchem Geschlecht identifizieren Sie sich? |
|                    | gender             | Man                                      | 2    |                       |                 |  Mann | |
|                    | gender             | Non-binary                               | 3    |                       |                 |  Nicht binär | | 
|                    | gender             | Other                                    | 4    |                       |                 |  Andere | | 
|                    | gender             | Not collected                            | -1   |                       |                 |  Nicht erhoben | |  
|                    | gender             | Prefer not to say                        | 0    |                       |                 |  Ich möchte keine Angaben dazu machen |  |
|  |  |  |  |  |  |  |  |
| Age                | age                | Age in years                             |      |  Age in years         | integer value   | Alter in Jahren | Alter in Jahren |
|  |  |  |  |  |  |  |  |
| Employment         | employment_status  | Full time employed                       | 1    |                       |                 | Vollzeit | Wie sind Sie beschäftigt? |
|                    | employment_status  | Employed part time                       | 2    |                       |                 | Teilzeit | |
|                    | employment_status  | Marginally employed (Minijob)            | 3    |                       |                 | Geringfügig beschäftigt (Minijob) | | 
|                    | employment_status  | Not employed but studying or in training | 4    |                       |                 | Nicht beschäftigt aber in Studium oder Ausbildung | |
|                    | employment_status  | Studying and employed                    | 5    |                       |                 | Studium und beschäftigt | |
|                    | employment_status  | Not employed                             | 6    |                       |                 | Nicht beschäftigt | |
|                    | employment_status  | Not collected                            | -1   |                       |                 | Nicht erhoben | |
|  |  |  |  |  |  |  |  |
| Preferred language | preferred_language | English                                  | 1    | What is the language you prefer to do the study in?* |   | Englisch | In welcher Sprache würden Sie gerne an dieser Studie teilnehmen? |
|                    | preferred_language | German                                   | 2    |                       |                 | Deutsch |
|                    | preferred_language | None of them                             | 3    |                       |                 | Keine von diesen |
|  |  |  |  |  |  |  |  |
| Preferred language proficiency (self-rated) | preferred_language_proficiency | Native       | 4 | How proficient are you in your preferred language? |  | Muttersprache | Wie gut beherrschen Sie Ihre bevorzugte Sprache? |
|                                             | preferred_language_proficiency | Advanced     | 3 |  |  | Fortgeschritten |  |  
|                                             | preferred_language_proficiency | Intermediate | 2 |  |  | Mittleres Niveau |  |
|                                             | preferred_language_proficiency | Basic        | 1 |  |  | Grundlegende Kenntnisse |  |
  


### Specific measurement instruments

| Description        | Variable           | Meaning                                  | Code | Question              | Notes           | Meaning German | Question German |
|--------------------|--------------------|------------------------------------------|------|-----------------------|-----------------|----------------|-----------------|
| Karolinska Sleepiness Scale (KSS) | kss | Extremely alert | 1 | Please rate your sleepiness in the last 5 minutes |  | Extrem wach | Bitte bewerten Sie Ihre Schläfrigkeit in den letzten 5 Minuten |
|                             | kss | Very alert      | 2 |  |  | Sehr wach |  |
|                             | kss | Alert           | 3 |  |  | Wach |  |
|                             | kss | Rather alert    | 4 |  |  | Ziemlich wach |  |
|                             | kss | Neither alert nor sleepy | 5 |  |  | Weder wach noch schläfrig |  |
|                             | kss | Some signs of sleepiness | 6 |  |  | Einige Anzeichen von Schläfrigkeit |  |
|                             | kss | Sleepy, but no effort to keep awake | 7 |  |  | Schläfrig, aber kann noch ohne Mühe wach bleiben |  |
|                             | kss | Sleepy, but some effort to keep awake | 8 |  |  | Schläfrig, habe Mühe wach zu bleiben |  |
|                             | kss | Very sleepy, great effort to keep awake, fighting sleep | 9 |  |  | Sehr schläfrig, kann nur mit großer Mühe wach bleiben; kämpfe gegen den Schlaf |  |
|                             | kss | Extremely sleepy, can't keep awake | 10 |  | Optional |  |  |

