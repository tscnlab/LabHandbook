# Folder structure

## Metadata

### Scope

The following presents a standardised way for naming and organising project code, materials and data. The level of this specification is at the level of folders and files, which exist on local drives, network drives, in repositories and in data releases (e.g. those on FigShare).

### Version

v1.0-20230517

### Owner

Manuel Spitschan

### Reviewer

Maydel Fernandez Alonso

## Definition

### Principles

The folder structure definition inherits several key naming conventions, including for [Participant ID](participant_id.md), and [Project Name](project_name.md).

### Definitions

A *visit* is each time a participant comes into the laboratory. This could include for example a screening visit.

An *experimental session* is a repeatable instance of a laboratoryu visit, such as a one-evening experiment. Each 

A *block* is repeatable instance of a collection of different tests.

A *test* is a repeatable test, e.g. saliva or PVT, questionnaires. A test can be a collection of trials.

Within a test, individual *trials* may occur, which are repeatable instance of a specific data collection unit, e.g. reaction time stimulus.

#### fMRI-specific definitions

Within the fMRI world, there are specific terms that we also use for consistency and clarity.

An *fMRI session* is a specific instance of participant entering the scanner.

Within an fMRI session, a participant will complete several runs, e.g. T1 structural scans or BOLD scans.

### Overall structure

The overall folder structure is defined as follows. The following are well-defined placeholders: $ProjectID, $ParticipantID. $_repo corresponds to the project-specific name of specific codes.

```
$ProjectID/
	ethics/
	code/		
	data/
		derivatives/ 
		raw/
			$ParticipantID/
	docs/
	notebooks/
	materials/
		questionnaires/
		sops/
	output/
	README.md
	reports/ 
		posters/
		presentations/
		manuscripts/
  
```

#### `README.md`

The file `README.md` contains information about the project, including the author.

#### `ethics` folder

The `ethics/` folder contains documentation about ethical approvals, including the full ethical application, approval letters and recruitment material. Any iterations of ethics should be included in this folder.

#### `code/` folder

The `code/` folder contains code used to run the experiment, analyse data, and other snippets of code to make the experiment reproducible. Depending on the project requirements, it is recommended to have separate GitHub repositories for different bits and pieces, e.g. separate out code to run the experiment from code to run the analysis. In any event, all code should be version-controlled on GitHUb.

#### `data/` folder

The `data/` folder contains all data collected in the project. This includes raw, processed and derived data. The `raw/` data folder is included to be organised by participants. Depending on the project needs, the folder structure of `derivatives` can be more loosely populated.

#### `docs/` folder 

The `docs/` folder contains documentation related to the project.

#### `notebooks/` folder 

The `notebooks/` folder contains computational notebooks related to the project, e.g. Jupyuter notebooks.

#### `materials/` folder 

The `materials/` folder contains questionnaires, SOPs and other materials to reproduce the data collectin effort.

#### `output/` folder 

The `output/` folder contains figures, tables and other data outputs related to the project.

#### `reports/` folder

The `reports/` folder contains any published outputs related to the project, including posters (in `posters/`), presentation decks (in `presentations/`) and manuscripts (`/manuscripts/`).