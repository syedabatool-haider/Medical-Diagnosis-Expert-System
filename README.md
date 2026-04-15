# Medical Diagnosis Expert System

A rule-based medical diagnosis expert system developed in **Prolog**.  
This project identifies possible diseases based on user symptoms and provides:

- possible disease prediction
- severity level
- confidence percentage
- matched symptoms
- recommended treatment
- preventive measures

## Project Overview

This expert system uses a knowledge base of symptoms and diseases to suggest the most likely illness for a patient.  
It compares the entered symptoms with stored disease symptoms and calculates a confidence score based on symptom matching.

The system currently includes diagnosis support for:

- Flu
- Common Cold
- Malaria
- COVID-19

## Features

- Rule-based diagnosis using Prolog
- Confidence percentage calculation
- Severity classification
- Suggested treatment for each disease
- Preventive measures for each disease
- Displays matched symptoms for justification

## Knowledge Base

The system contains:

- symptoms such as fever, cough, sore throat, fatigue, body ache, chills, loss of smell, headache, nausea, and sweating
- diseases including flu, common cold, malaria, and covid19
- severity levels: mild, moderate, and severe
- treatment recommendations
- preventive measures

## How It Works

The system works by:

1. taking a list of patient symptoms
2. comparing them with the symptoms of each disease
3. calculating a confidence percentage
4. sorting possible diseases by confidence and severity
5. returning the most likely disease with explanation, treatment, and prevention advice

## Main Predicates

- `confidence(Disease, PatientSymptoms, ConfidencePercent, MatchedSymptoms)`
- `possible_diseases(PatientSymptoms, Results)`
- `diagnose(PatientSymptoms, Disease, Recommendation)`
- `treatment_for(Disease, Treatment)

## How to Run

Open the file in a Prolog environment such as **SWI-Prolog**.
Load the file:
```prolog
['main.pl'].
