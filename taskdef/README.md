# SEEDUtils

### Data Format

| Category | Task | Input | Output | Task Definition |
|------|---------|----------------|----------------| -------------- |
| Evaluation  |  Code Generation   |  text or code  |  scores   |  A library for software engineering task evaluation |
|  Consistency | SEEDConsistencyChecker| code | scores | Check the consistency of code |
| Poison | Preprocess Dataset | Datasets in .jsonl.gz format (path to dir) | null | Initiates preprocessing for the attack |
| Poison | Poison Dataset | Dataset in .jsonl format | null | Poisons the dataset with BADCODE |


