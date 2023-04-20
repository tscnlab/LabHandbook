

# Terminology

## Terms for generic projects

| Term                 | Definition                                                                                                  |
|----------------------|-------------------------------------------------------------------------------------------------------------|
| Visit                | Participant comes in the laboratory, irrespective of purpose (e.g. experimental procedure, screening, etc.) |
| Experimental session | Repeatable instance of laboratory entry, e.g. participant enters the laboratory for 6 hours                 |
| Block                | Repeatable instance of a collection of different tests                                                      |
| Test                 | Repeatable test (e.g. saliva, PVT, questionnaires, etc.)                                                    |
| Trial                | Repeatable instance of a specific data collection unit (e.g. reaction time stimulus)                        |

## fMRI specific terms

| Term                 | Definition                                                                                                  |
|----------------------|-------------------------------------------------------------------------------------------------------------|
| Session              | Instance of participant entering the scanner                                                                |
| Run                  | Different acquisition run, e.g. T1 image or EPI                                                             |
| Block                | Period of time during which a specific stimulus or task is presented to the participant; long enough to allow for stable brain activation patterns to emerge, typically lasting between 10 and 30 seconds                                                           |


Within a block, you can have an fMRI session, which contains different runs

# Naming conventions

* Project ID
* Central participant ID
* (Project-specific) Participant ID


## Project ID

* `<Project abbreviation>_<Instance number>`
* Examples
    - BinIntMlt01 - Binocular integration in melatonin suppression
    - CiViBe01
    - CiViBrain01
    - SpTmpMlt01
    - ReWoCap01



* Comma-separated entries for multiple items for metadata
    - Project abbreviation, Long format name, Responsible owner, Ethical approval number, Team members, Tests, Start date, End date, Data collection code repository, Analysis code repository, Supplementary code repository, Archival data repositories, Pre-registration DOI, Preprint DOI, Publication DOI





## Central participant ID

* `<Year of first entry><Running number>`
    - Number assigned at consent

* Examples
    ```bash
    220001
    220002
    220005
    ```




## Project-specific participant ID

* `<Year of first entry><Running number>`
    - Number assigned at consent
* Examples

    ```bash
    101
    102
    103
    ```



* Examples

    | central_pid | project_name | project_pid |
    |-------------|--------------|-------------|
    | 220005      | BinIntMel    | 101         |
    | 220006      | CiViBe       | 104         |


    - When participant is coming, have they already participated?
    - Consent form "data base" with Central ID written on the form
    - Confirm with participant if they already have participated
    - Add project to central data base

