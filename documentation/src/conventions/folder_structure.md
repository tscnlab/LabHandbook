### ADDED TO DEMONSTRATE

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

The `data/` folder contains all data collected in the project. This includes raw, processed and derived data. The `raw/` data folder is included to be organised by participants. Depending on the project needs, the folder structure of `derivatives` can be more loosely populated. We consider derivatives data that are one step away from the raw data, e.g. manually cleaned or preprocessed data.

Data in in the `data/` folder follow the following pattern:

```
$ProjectID/data/<processing step>/$ParticipantID/<session number>_expsession/<modality>/<block number>_<tests>[-<test number>]_<timestamp>.<file_extension>
```

The `data/raw/` folder is organised with the following subfolders:

```
data/raw/screening/
data/raw/continuous/
data/raw/expsession01/
data/raw/expsession02/
data/raw/expsession03/
...
data/raw/expsession##/

```

As an example:

```
CiViBe/
	data/ <- Check
		derivatives/ 
		raw.csv (database of measurements, NT)
		raw/ <- Check
			101
				Screening/ <- 
					metropsis/
						01_metropsis_<timestamp>/
					oct/	
						01_oct_<timestamp>/
								01_oct_<timestamp>.metadata.txt
								01_oct_<timestamp>.dicom
								01_oct_<timestamp>.csv
				Continuous/
					metadata.txt
					actigraphy/
						01_actigraphy_<timestamp>.txt
					  01_actigraphy_<timestamp>.metadata.txt
					sleepdiary/
						01_sleepdiary_<timestamp>.txt
						01_sleepdiary_<timestamp>.metadata.txt
				01_expsession/ <- Experimental session
					log_<timestamp>.log <- Check (session-wise log)
					metadata.txt <- Experimental meta-data
					resources/ <- Optional
						00_beep.wav
						00_stimulus_sequences.csv
					pvt/
						01_pvt01_<timestamp>.csv <- Check if block is 2 numbers, then string, then timestamp
		        01_pvt01_<timestamp>.csv
						01_pvt01_<timestamp>.log (test-wise log) <- Optional
						01_pvt01_<timestamp>.log (test-wise log)
					oct/			
						<block>_<test>-<number>_<timestamp>.<filetype>		
						01_cornealthickness_<timestamp>.metadata.txt
						01_cornealthickness_<timestamp>.dicom
						01_cornealthickness_<timestamp>.csv
						01_macula_<timestamp>.metadata.txt
						01_macula_<timestamp>.dicom
						01_macula_<timestamp>.csv
						02_macula_<timestamp>.metadata.txt
						02_macula_<timestamp>.dicom
						02_macula_<timestamp>.csv
```


The `screening` folder contains all information related to the screening session. 

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
