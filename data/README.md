### Data folder

The data directory contains data used in the analysis. This is treated as read only; in paricular the R/python files are never allowed to write to the files in here. Depending on the project, these might be csv files, a database, and the directory itself may have subdirectories.

+ ``train_target_sub3840.npy``: Our subsetted target dataset.
+ ``train_input_sub3840.npy``: Our subsetted input dataset.
