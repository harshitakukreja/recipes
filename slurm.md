# Allocate resources and attach terminal
```bash
salloc --partition=dgx --time=04:00:00 --gres=gpu:1 --mem=200G
srun --pty /bin/tcsh # will enter into some terminal
pwd
conda activate ./.conda
python ...
```

# Directy run
```bash
conda activate ./.conda
srun --job-name=<job_name> --partition=dgx --time=04:00:00 --gres=gpu:1 --mem=200G python ...
```

# List all jobs
```bash
squeue -u <user_name>
```

# Kill a job
```bash
scancel <job_id>
```
_NOTE_: Get `<job_id>` from `squeue`
