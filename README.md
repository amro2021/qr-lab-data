# QR Lab data

Measurement datasets from the QR Multiplex Lab receiver
(https://amro2021.github.io/qr-transfer/multi/ → Receive → **Save new runs to GitHub**).

* `data/` one `.zip` per save, named `<phone name>-<UTC time>.zip`
* `results/` figures, tables and a summary, rebuilt automatically from all datasets each time a new one arrives
  (see [results/README.md](results/README.md))

The analysis code lives in [amro2021/qr-transfer](https://github.com/amro2021/qr-transfer/tree/main/analysis).
This repository is kept separate so that the upload token given to receivers can only add data here and cannot
change the website. Every change is kept in the git history, so a deleted or overwritten dataset can be restored.
