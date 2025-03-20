## ULS23 Baseline Model Container
This folder contains the code to build a GrandChallenge algorithm out of the faster version of the ULS baseline model.

- `/architecture/extensions/nnunetv2` contains the extensions to the nnUNetv2 framework that should be merged with your local install.
- `/architecture/nnUNet_results/` should contain the baseline (or your own) nnUNet model weights and plans file.
- `/architecture/input/` contains an example of a stacked VOI image and the accompanying spacings file. Uncommenting line 64 in the Dockerfile will allow you to run your algorithm locally with this data and check whether it runs inference correctly.
- `train_test_split.json` contains the train/test split used for evaluation of the baseline model on the training datasets, use it if you want to reproduce our results.
