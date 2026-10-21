# QR Lab Results

3 runs, 1240 processed frames and 375 QR reads from 1 dataset file(s). Updated 2026-10-21 19:51 UTC.

| Scheme | Distance (m) | Runs | Frame loss | Module errors | Completion (s) | Goodput (B/s) |
|---|---:|---:|---:|---:|---:|---:|
| Layered a=170 | 0.1 | 2 | 38.7 % | 9.0e-02 | – | – |
| nan | 0.1 | 1 | – | – | – | – |

### Frame loss per stream vs distance (mean ± 95 % CI over runs).

![Frame loss per stream vs distance (mean ± 95 % CI over runs).](fig_frame_loss_by_stream.png)

[PDF](fig_frame_loss_by_stream.pdf)

### Raw module error rate before QR error correction. Open markers: no errors measured.

![Raw module error rate before QR error correction. Open markers: no errors measured.](fig_module_error_rate.png)

[PDF](fig_module_error_rate.pdf)

### Share of processed camera frames in which each stream was read.

![Share of processed camera frames in which each stream was read.](fig_success_per_frame.png)

[PDF](fig_success_per_frame.pdf)

### Fraction of blocks recovered over time, one line per run.

![Fraction of blocks recovered over time, one line per run.](fig_progress.png)

[PDF](fig_progress.pdf)

Tables: [summary_by_scheme.csv](summary_by_scheme.csv) · [summary_by_scheme.tex](summary_by_scheme.tex) · [summary_by_stream.csv](summary_by_stream.csv) · [METHODS.md](METHODS.md)
