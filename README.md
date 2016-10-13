# Running submiterator in batch mode
Scripts for posting batches of HITs to MTurk via [Submiterator](https://github.com/feste/Submiterator)

# Usage

### To post batches of experiments:

`./post_batches.sh nameOfExpt nBatches nTurkersPerBatch`

- `nameOfExpt`: a string, name of the folder inside which lives `nameOfExpt.config` [see [submiterator for details](https://github.com/feste/Submiterator)]
- `nBatches`: the number of batches to run
- `nTurkersPerBatch`: the number of turkers you want for each batch (note, if you the number of turkers per batch is 9 or fewer, you avoid the +20% mturk fee)

### To get batches of experiments:

`./get_batches.sh nameOfExpt`

### To merge the data (or invoices, subject information, etc.)

File `merge_invoices.R` should be run inside R. (need to edit the details of the file)