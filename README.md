## R CI with Azure Pipelines

CI on **R 3.6** or above.

Platforms - *Linux*, *macOS*, and *Windows*

To use this add followings to your `azure-pipelines.yml`
```yaml
resources:
  repositories:
    - repository: r-azure-pipelines
      type: github
      name: orgdb/r-azure-pipelines
      endpoint: orgdb

jobs:
    - template: azure-tidyverse.yml@r-azure-pipelines
```
