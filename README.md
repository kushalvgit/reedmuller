# reedmuller

## Subspaces Folder Description

This folder contains all the subspace (coset) configurations used in our simulations. Each file represents a specific set of subspaces chosen for decoding Reed–Muller codes, and the naming convention reflects key parameters used during the experiments.

### File Naming Convention

m<M>_<type><spread>_<num>.txt


Where:

- `m<M>`: Indicates the dimension of the RM code (e.g., `m8` for RM codes with `m = 8`)
- `<type>`: Specifies the selection strategy for subspaces:
  - `dis`: Subspaces were selected based on *disjoint* cosets
  - `ran`: Subspaces were selected *randomly*
- `<spread>`: Indicates the spread configuration:
  - `1` or `2` refer to how many different spreads were used
- `<num>`: The final number denotes:
  - For `dis` files: the **number of subspaces** selected
  - For `ran` files: the **correlation threshold** used during selection

### Examples

- **`m8_1dis_spread1_85.txt`**  
  → 85 subspaces selected from a single spread for `m = 8`.  
  The `1dis` indicates that the subspaces come from one disjoint spread.

- **`m9_3dis_spread1_493.txt`**  
  → 493 subspaces selected from three disjoint spreads for `m = 9`.

- **`m8_ran1_85_225.txt`**  
  → Randomly selected subspaces for `m = 8`, with a correlation threshold of 225.  
  The file includes 85 subspaces chosen using `ran1` configuration.

