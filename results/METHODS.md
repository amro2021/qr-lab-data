# Measurement summary

Dataset: 7 runs, 2167 processed camera frames, 381 QR codes read,
377 codes with raw module-error measurements,
2 receiving device(s). Schemes: Layered a=170, Per-user 2 tiles, Per-user color.

## Metric definitions

* **Frame loss** (per stream): every QR code carries the sender frame counter k. For a stream,
  frame loss = 1 − (distinct k read) / (k_max − k_min + 1), averaged over the streams of a run.
  It includes sender frames the camera never sampled; compare the receiver processing rate
  (runs.proc_fps) with the sender frame rate (runs.sender_fps).
* **Success per processed frame**: fraction of processed camera frames in which the stream was read.
* **Module error rate (MER)**: the decoded text is re-encoded with the same QR library and
  error-correction level as the sender, which reproduces the transmitted module matrix exactly; each
  module centre of the binary image given to the decoder is compared with it. This is a raw,
  pre-Reed–Solomon symbol error rate, conditional on the code having been located and decoded.
* **Completion time T_c**: time from the first QR code of a file to its SHA-256-verified reconstruction
  (maximum over the files of a run).
* **Goodput**: delivered file bytes / T_c.
* **Reception overhead ε**: (unique packets needed) / K − 1 for the LT fountain code (Robust Soliton,
  c = 0.1, δ = 0.5, systematic first K packets).
* Confidence intervals: 95 % Student-t intervals over repeated runs at the same scheme and distance.
