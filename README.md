\# Topology Inference Accuracy in Narrowband PLC Under Variable Distributed Generation Penetration



Research project for submission to IEEE ICC 2027 (SAC: Smart Grid Communications).



\## Authors

\- Matheus Lopes Ferreira da Costa — Electrical Engineering (Power Systems)

\- Clara Mayan Marin Quispe — Telecommunications Engineering



\## Structure



\- `feeder/` — IEEE 13-Node Test Feeder OpenDSS files

\- `notebooks/electrical/` — power system simulation (OpenDSS, DG scenarios, losses, impedance)

\- `notebooks/telecom/` — PLC channel model and topology inference classifier

\- `data/electrical/` — CSV outputs from the electrical simulation (handoff files)

\- `data/telecom/` — CSV outputs from the channel model and classifier

\- `figures/electrical/` — plots generated from the electrical simulation

\- `figures/telecom/` — plots generated from the channel model and inference results

\- `docs/` — research notes and planning documents



\## Pipeline



1\. Electrical simulation (OpenDSS via opendssdirect) generates voltage, distance, impedance, and losses per bus, per DG penetration scenario, per hour.

2\. Handoff files in `data/electrical/` feed the PLC channel model.

3\. Telecom notebook computes CIR/CTF per node/scenario and trains a topology inference classifier.



\## Deadline

IEEE ICC 2027 submission deadline: October 2, 2026.

