# Workflow

### 1. Load Data
- Call the fileAligner to get both the patient information file and the methylation data for the respective patients.

### 2. Distinguish Phentotype Groups
- Separate into the the groups of each phenotype you wish to investigate the cell type fractions for.

### 3. Run CellDMC
- Input the methylation data (n_samples, n_features), list of phenotypes (n_samples), and fraction (n_samples x n_features).

### 4. Extract Cell-specific CpG Sites
- For each cell type collect their corresponding DMCTs if present.

### 5. Calculate Coefficients
- Run through elastic net regularization model to find coefficients.

### 6. Calculate Cell Age
- Run coefficients & methylation data through Horvath Clock.
