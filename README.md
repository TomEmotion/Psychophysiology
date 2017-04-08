# Psychophysiology
LabVIEW-based software for psychophysiology analysis

Currently this project involves VIs for the preprocessing and analysis of Skin Conductance data. Electromyography, cardiac and respiratory analysis will be added.

SCR Analysis
OS: This LabVIEW VI and library can be built into a standalone executable that runs under Windows, with versions for OSX and Linux on the way.

Summary
The software allows for analysis of event-locked and spontaneous skin conductance responses (SCRs). Data can be imported in the form of CSV/tab delimited text files with a single column for SCR data. Additional columns can contain time information and event markers. Sample rate will be read from time information, or can be specified by the user. Event markers can be used for event-related analysis; alternatively, separate tab delimited text timing files can be provided.

Preprocessing options include user-specified bandpass filtering, median filtering and sample rate conversion.

Analysis is based on a linear modeling approach using a set of basis functions to model SCRs. Currently options exist for block, tent, and Fourier basis sets. 

Output includes mean estimated responses per condition, as well as basis set weights per condition.
