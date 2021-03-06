---
jupytext:
  cell_metadata_filter: -all
  formats: md:myst
  text_representation:
    extension: .md
    format_name: myst
    format_version: 0.13
    jupytext_version: 1.11.5
kernelspec:
  display_name: Python 3
  language: python
  name: python3
---

# Data Sources

The project uses numerous data sources from North Bristol NHS Trust (NBT), with the aim of using available data to facilitate the development of multi-modal models. This page explores the sources of data that are available and explains how they will be used in the project. 

<h3> North Bristol Trust Data Warehouse </h3>

The project uses an extract of data held at the NBT Data Warehouse from a 15 year period. The data held includes Electronic Patient Record (EPR) data fields, which are extracted from the Trust's "Lorenzo" computer system, and contains data fields such as NHS Number  which are used to link data between sources. The NBT Data Warehouse also contains data fields from the Radiology Information System (RIS), which includes details of the procedures and examinations undergone by patients. Diagnosis codes (ICD-10 Codes) are also stored in the Data Warehouse, which are used in patient selection to identify patients diagnosed with stroke. 

<h3> SSNAP </h3>

Patients who have been diagnosed with stroke have their data entered into a nationwide database called Sentinel Stroke National Audit Programme (SSNAP). As this database only contains records of patients who have been diagnosed with stroke, these records alongside ICD-10 codes from the NBT Data Warehouse can be used to identify diagnoses.

<h3> PACS </h3>

Picture Archiving and Communication System (PACS) is the system used by NBT to store imaging data. This system is therefore used to access the images created as a result of procedures such as CT scans, MRI scans and angiograms. The format used to store and transfer image files in PACS is called "Digital Imaging and Communication in Medicine" (DICOM). 

<h3> Data Workflow </h3>

The figure below shows the data flows and process for this project, including pseudonymisation and anonymisation.

<img src="workflow.*" width = "800" height = "400">