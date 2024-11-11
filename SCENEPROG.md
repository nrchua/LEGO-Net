# Setup
- Clone repository
- Run `setup.sh`
- Download the [3DFRONT_65347.zip](https://drive.google.com/drive/folders/1MmSb6461ixGGqGa5hRY3s0IR4xTeRdPF) and extract in the parent directory
- Download [Chair.h5](https://drive.google.com/drive/folders/1MmSb6461ixGGqGa5hRY3s0IR4xTeRdPF) and [Table.h5](https://drive.google.com/drive/folders/1MmSb6461ixGGqGa5hRY3s0IR4xTeRdPF) and place them within a new directory at `./ConDor_torch/preprocessed_condor_output`
- Download [bedroom checkpoint](https://drive.google.com/file/d/183j3i6R-YtgyOkWsUYnH894ZBkdyseZH/view) [living room checkpoint](https://drive.google.com/file/d/1FKkjaKHC5alrN3SsPDAZ3iU24AfAEw4s/view) or and place in a folder called `./checkpoints`
- Within `./3DFRONT_65347/processed_bedroom_augmented` or `./3DFRONT_65347/processed_livingroom_augmented`, place your `sceneprog_dataset.npz` data file -- containing the arrays necessary
- In `filepath.py`, set the `home_dir` variable to the parent directory (ex: `home_dir="/nick-data/sceneprog/LEGO-Net"`)
- When ready to run, activate the venv `source ./sceneprog/bin/activate`
- Then call `./inference.sh` to begin inference. Results will be saved in `./checkpoints`