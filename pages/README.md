## About

To support research on Trace Amine-Associated Receptors (TAARs) and their role in sleep-wake regulation, the Sleep Neurobiology Laboratory at SRI International provides this dataset on TAAR2-9 knockout (KO) mice. The data are intended to facilitate investigation into the physiological and neurobiological impacts of TAAR family members on sleep structure, EEG spectral power, and dopaminergic signaling.

## Methods

This dataset comprises physiological recordings from male TAAR2-9 KO and wild-type (WT) C57BL/6J mice. Recordings were collected under baseline, sleep deprivation, and pharmacological conditions.

Signals measured include:

- EEG (electroencephalogram)
- EMG (electromyogram)
- Locomotor activity (LMA)
- Subcutaneous body temperature (Tsc)

Cohorts:

- Batch 1: 8 KO mice (mouse 3–6, 8–12) and 3 WT mice (mouse 1, 2, 7).
- Batch 2: 9 WT mice (mouse 1–9).

**1. Animals**

TAAR2-9 Knockout (KO) Mice:

- Male TAAR2-9 KO mice (n = 8) on a pure C57BL/6 background.
- Knockout (KO) Mice used:
	- 6hSD: mouse3–6, mouse8–11
	- Baseline: mouse3–6, mouse8–12
	- Dosing: : mouse3–6, mouse8–11
- Wild-Type (WT) Controls:
	- 6hSD
		- mouse1, mouse2, mouse7- Batch 1
		- mouse 1-9 – Batch2
	- Baseline
		- mouse1, mouse2, mouse7- Batch 1
		- mouse 1-9 – Batch 2

Housing Conditions:

- Group-housed under a 12h:12h light-dark cycle before surgery and singly-housed after transmitter implantation.

**2. Surgical Procedures**

- Mice were implanted with wireless HD-X02 transmitters (DSI, Inc., St. Paul, MN) to record EEG/EMG
- Transmitters were placed in a subcutaneous pocket created in right dorsal flank.
- EEG leads targeted the hippocampus and cerebellum; EMG leads were sutured to the neck
muscle.
- Postoperative analgesia was administered for 2–3 days.

**3. Experimental Design**

Recordings were structured into four main protocols:

- Baseline Sleep/Wake Recording: 25-h continuous EEG/EMG recording starting at ZT23.
- Multiple Sleep Latency Test (mMSLT):
	- Beginning at ZT3, 5 trials of 20 min SD interspersed with 20 min recovery periods
- Pharmacology:
	- Oral administration at ZT6 of:
		- Vehicle (10% DMSO),
		- TAAR1 partial agonist RO5263397 (1 mg/kg),
		- TAAR1 full agonist RO5256390 (3 or 10 mg/kg),
		- Caffeine (10 mg/kg, positive control).
	- At least 72 h washout between sessions.
- Sleep Deprivation:
	- 6h SD: ~12h continuous EEG/EMG recording starting at ZT23

**Summary of Findings**

- TAAR2-9 KO mice showed:
	- Decreased wakefulness and increased REM and NREM sleep.
	- Sleep fragmentation: more REM bouts, shorter wake and REM durations.
	- Elevated dopaminergic activity (increased TH+ cells in VTA).
	- TAAR1 agonists reduced REM sleep; caffeine promoted wakefulness as expected.

## Data overview

**Approved users can browse and [download the TAAR2-9 knockout (KO) mice data here](:files_path:).**

The repository contains both EDF (raw signals) and FFT (spectral analysis) files, organized under the following experimental conditions:

- Baseline
- Dosing
- Sleep Deprivation
	- 6-hour SD (6hSD)
	- Multiple Sleep Latency Test (mMSLT)

For Dosing experiments, only KO mice (mouse 3–6, 8–11) were analyzed in the published paper. Data from low signal-to-noise mice (e.g., mouse 12) were excluded.

**Mouse Identification**

- Each file name includes the mouse identifier (e.g., mouse01 or mouse1).
- For dosing data, files are named as DosingX_mouseY, where X = dosing number and Y = mouse number.

**Folder Structure**

[/edf](:files_path:/EDF files): Exported EDF files from Ponemah/Neuroscore™ systems containing raw signals:

- EEG, EMG, temperature (Tsc), signal strength, and locomotor activity (LMA).
- Sampling rates:
	- EEG/EMG: 500 Hz
	- Tsc and signal strength: 10 Hz
	- Activity: 1 Hz
- Transmitters: DSI HD-X02 wireless telemeters

[/fft](:files_path:/FFT files): CSV files containing:

- Power spectral density (PSD) values
- Sleep state scoring across 10-second epochs
- FFT range: 0–100 Hz in 0.122 Hz bins

## Access and usage restrictions

The TAAR2-9 knockout (KO) mice dataset is only available for non-commercial use.

## Citation and acknowledgement

When using this dataset, users must cite the following:

> [Zhang GQ, Cui L, Mueller R, Tao S, Kim M, Rueschman M, Mariani S, Mobley D, Redline S. The National Sleep Research Resource: towards a sleep data commons. J Am Med Inform Assoc. 2018 Oct 1;25(10):1351-1358. doi: 10.1093/jamia/ocy064. PMID: 29860441; PMCID: PMC6188513.](https://pubmed.ncbi.nlm.nih.gov/29860441/)
>
> [Park S, Heu J, Scheldrup G, Tisdale RK, Sun Y, Haire M, Ma SC, Hoener MC, Kilduff TS. Trace amine-associated receptors (TAARs)2-9 knockout mice exhibit reduced wakefulness and disrupted REM sleep. Front Psychiatry. 2025 Jan 29;15:1467964. doi: 10.3389/fpsyt.2024.1467964. PMID: 39944134; PMCID: PMC11814429.](https://pubmed.ncbi.nlm.nih.gov/39944134/)

Users must include the following text in any Acknowledgements:

> The recordings deposited here were supported by NIH R01NS103529 and R01NS136808 to Thomas S. Kilduff. The National Sleep Research Resource was supported by the U.S. National Institutes of Health, National Heart Lung and Blood Institute (R24 HL114473, 75N92019R002).

## Changelog

*September 2025*

- Make TAAR2-9 knockout (KO) mice dataset available for data requests

## References

- TAAR2-9 knockout (KO) mice GitHub Documentation: https://github.com/nsrr/taar2-9-knockout-mice-documentation

## Questions?

Please reach out to us at support@sleepdata.org or in the [Forum](https://sleepdata.org/forum) if you have questions.
