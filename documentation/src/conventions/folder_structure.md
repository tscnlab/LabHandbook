# Folder structure

## Scope

The following presents a standardised way for naming and organising project code, materials and data. The level of this specification is at the level of folders and files, which exist on local drives, network drives, in repositories and in data releases (e.g. those on FigShare).

## Definition

### Principles

The folder structure definition inherits several key naming conventions, including for [Participant ID](participant_id.md), [Project Name](project_id.md) and [Timestamps](timestamps.md).

### Definitions

An *experimental session* is a repeatable instance of a laboratory visit, such as a one-evening experiment. Each experimental session will have its own folder named `##_expsession`, where `##` is the running number. We consider screening visits an experimental session and place them in the `screening` folder. There are also data modalities that do not conform to this definition of a session, e.g. actigraphy or sleep diary measurements, which cannot be linked to a specific session. These are 

A *block* is repeatable instance of a collection of different tests.

A *test* is a repeatable test, e.g. saliva or PVT, questionnaires. A test can be a collection of trials.

Within a test, individual *trials* may occur, which are repeatable instance of a specific data collection unit, e.g. reaction time stimulus.

#### fMRI-specific definitions

Within the fMRI world, there are specific terms that we also use for consistency and clarity.

An *fMRI session* is a specific instance of participant entering the scanner.

Within an fMRI session, a participant will complete several runs, e.g. T1 structural scans or BOLD scans.

### Overall structure

The overall folder structure is defined as follows. The following are well-defined placeholders: `$ProjectID`, `$ParticipantID`. `$_repo` corresponds to the project-specific name of specific codes.

```
$ProjectID/
	ethics/
	code/
		$_repo		
	data/
		derivatives/
		outputs/
		raw.csv
		raw/
			$ParticipantID/
	docs/
	materials/
		questionnaires/
		sops/
	outputs/
	README.md
	reports/ 
		posters/
		presentations/
		manuscripts/
  
```

Note that each project folder is linked to one specific project and is self-contained. If there are multiple versions of an experiment or a pilot data collection, this should be represented in the hierarchy by including it at the participant-level, e.g. as follows:

```
data/raw/101/pilot
data/raw/101/main_expt
```

#### `README.md`

The file `README.md` contains information about the project, including the author.

#### `ethics` folder

The `ethics/` folder contains documentation about ethical approvals, including the full ethical application, approval letters and recruitment material. Any iterations of ethics should be included in this folder.

#### `code/` folder

The `code/` folder contains code used to run the experiment, analyse data, and other snippets of code to make the experiment reproducible. Depending on the project requirements, it is recommended to have separate GitHub repositories for different bits and pieces, e.g. separate out code to run the experiment from code to run the analysis. In any event, all code should be version-controlled on GitHub.

The `code/` folder may also include notebooks for reproducible analyses, e.g. Jupyter notebooks.

#### `data/` folder

The `data/` folder contains all data collected in the project. This includes raw, processed and derived data. The `raw/` data folder is included to be organised by participants. Depending on the project needs, the folder structure of `derivatives` can be more loosely populated. We consider derivatives data that are one step away or multiple steps from the raw data, e.g. manually cleaned or preprocessed data. The `outputs/` folder contains any outputs directly generated from the data that are useful but not meant for publication.

Data in in the `data/` folder follow the following pattern:

```
$ProjectID/data/<processing step>/$ParticipantID/<experiment name (e.g. pilot or main)>/<session number>_expsession/<modality>/<block number>_<tests>[-<test number>]_<timestamp>.<file_extension>
```

The `raw.csv` file contains an overview of the data collected and available in the `data/` folder. This is to keep an inventory of the data collected.

The `data/raw/` folder is organised with the following subfolders:

```
data/raw/main/screening/
data/raw/main/continuous/
data/raw/main/01_expsession/
data/raw/main/02_expsession/
data/raw/main/03_expsession/
...
data/raw/main/##_expsession##/
data/raw/main/group/
```

Here, `main` corresponds to the main experiment, but could also be e.g. `pilot`.

The `group/` folder contains any data that are collected and only available at the group level and not at the individual-participant level. This includes, for example, data from REDCap or from devices that only collect data from multiple participants.

As an example:

```
CiViBe/
	data/
		derivatives/ 
		raw/
			101
				main/
					screening/ 
						metropsis/
							01_metropsis_<timestamp>/
						oct/	
							01_oct_<timestamp>/
									01_oct_<timestamp>.metadata.txt
									01_oct_<timestamp>.dicom
									01_oct_<timestamp>.csv
					continuous/
						metadata.txt
						actigraphy/
							01_actigraphy_<timestamp>.txt
							01_actigraphy_<timestamp>.metadata.txt
						sleepdiary/
							01_sleepdiary_<timestamp>.txt
							01_sleepdiary_<timestamp>.metadata.txt
					01_expsession/
						log_<timestamp>.log <- Check (session-wise log)
						metadata.txt <- 



						meta-data
						resources/ <- Optional
							00_beep.wav
							00_stimulus_sequences.csv
						pvt/
							01_pvt01_<timestamp>.csv <- Check if block is 2 numbers, then string, then timestamp
						01_pvt01_<timestamp>.csv
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

Timestamps follow the [Timestamps](timestamps.md) convention.

#### `docs/` folder 

The `docs/` folder contains documentation related to the project.

#### `materials/` folder 

The `materials/` folder contains questionnaires, SOPs and other materials to reproduce the data collectin effort.

#### `outputs/` folder 

The `outputs/` folder contains figures, tables and other data outputs related to the project that will be used in publications and other external documents. Note that the `data/` folder also contains an `outputs/` folder which contains intermediate figures.

#### `reports/` folder

The `reports/` folder contains any published outputs related to the project, including posters (in `posters/`), presentation decks (in `presentations/`) and manuscripts (`/manuscripts/`).


### Creating an empty structure

To create an empty folder, you can run the following commands in Terminal (OS X & Linux):

```
mkdir EMPTY_PROJECT
mkdir EMPTY_PROJECT/ethics
mkdir EMPTY_PROJECT/code
mkdir EMPTY_PROJECT/data
mkdir EMPTY_PROJECT/data/derivatives
mkdir EMPTY_PROJECT/data/raw
mkdir EMPTY_PROJECT/data/raw/101
mkdir EMPTY_PROJECT/data/raw/101/screening
mkdir EMPTY_PROJECT/data/raw/101/continuous
mkdir EMPTY_PROJECT/data/raw/101/01_expsession
mkdir EMPTY_PROJECT/data/raw/101/01_expsession/meas/
mkdir EMPTY_PROJECT/docs
mkdir EMPTY_PROJECT/notebooks
mkdir EMPTY_PROJECT/materials
mkdir EMPTY_PROJECT/materials/questionnaires
mkdir EMPTY_PROJECT/materials/sops
mkdir EMPTY_PROJECT/outputs
touch EMPTY_PROJECT/README.md
```
