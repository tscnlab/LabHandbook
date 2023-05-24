# Variables

## Scope

The following presents a standardised way for naming variables and their response options, specifically arising from questionnaires and surveys.

## Definition

We agreed to use the following conventions for demographic variables and answer possibilities and the for the Karolinska Sleepiness Scale (KSS) (10 is optional):

The option "Prefer not to say" is always the last option in single choice answers.
The option "Not collected" is not provided as a choice to select, this is an internal coding.
* For "Preferred language" the following note has to be added to the question:
"Note: If you do not prefer either of the languages, you are not eligible for the study.
       This means you can not participate in the study."



| Description        | Variable           | Meaning                                  | Code | Question              | Notes           |
|--------------------|--------------------|------------------------------------------|------|-----------------------|-----------------|
| YesNo              | yesno              | Yes                                      | 1    |                       | binary question |
|                    | yesno              | No                                       | 0    |                       |                 |
| Sex                | sex                | Female                                   | 1    | Sex assigned at birth |                 |
|                    | sex                | Male                                     | 2    |                       |                 |
|                    | sex                | Intersex                                 | 3    |                       |                 |
|                    | sex                | Not collected                            | -1   |                       |                 |
|                    | sex                | Prefer not to say                        | 0    |                       |                 |
| Gender             | gender             | Woman                                    | 1    |                       |                 |
|                    | gender             | Man                                      | 2    |                       |                 |
|                    | gender             | Non-binary                               | 3    |                       |                 |
|                    | gender             | Other                                    | 4    |                       |                 |
|                    | gender             | Not collected                            | -1   |                       |                 |
|                    | gender             | Prefer not to say                        | 0    |                       |                 |
| Age                | age                | Age in years                             |      |  Age in years         | integer value   |
| Employment         | employment_status  | Full time employed                       | 1    |                       |                 |
|                    | employment_status  | Employed part time                       | 2    |                       |                 |
|                    | employment_status  | Marginally employed (Minijob)            | 3    |                       |                 |
|                    | employment_status  | Not employed but studying or in training | 4    |                       |                 |
|                    | employment_status  | Studying and employed                    | 5    |                       |                 |   
|                    | employment_status  | Not employed                             | 6    |                       |                 |
|                    | employment_status  | Not collected                            | -1   |                       |                 |
| Preferred language | preferred_language | English                                  | 1    | What is the language you prefer to do the study in?* |   |
|                    | preferred_language | German                                   | 2    |                       |                 |
|                    | preferred_language | None of them                             | 3    |                       |                 |
| Preferred language proficiancy (self-rated) | preferred_language_proficiency | Native       | 4 |  |  |
|                                             | preferred_language_proficiency | Advanced     | 3 |  |  |
|                                             | preferred_language_proficiency | Intermediate | 2 |  |  |
|                                             | preferred_language_proficiency | Basic        | 1 |  |  |
|  |  |  |  |  |  |
| Karolinska Sleepiness Scale (KSS) | kss | Extremely alert | 1 |  |  |
|                             | kss | Very alert      | 2 |  |  |
|                             | kss | Alert           | 3 |  |  |
|                             | kss | Rather alert    | 4 |  |  |
|                             | kss | Neither alert nor sleepy | 5 |  |  |
|                             | kss | Some signs of sleepiness | 6 |  |  |
|                             | kss | Sleepy, but no effort to keep awake | 7 |  |  |
|                             | kss | Sleepy, but some effort to keep awake | 8 |  |  |
|                             | kss | Very sleepy, great effort to keep awake, fighting sleep | 9 |  |  |
|                             | kss | Extremely sleepy, can't keep awake | 10 |  | Optional |

