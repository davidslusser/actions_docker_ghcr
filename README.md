# actions_docker_ghcr
A Github action for building a Docker image and pushing to Github Container Registry.

<br/>


## How to use 
In your .github/workflows directory, create a yaml file (such as main.yaml). Add a job for each desired workflow with the `uses` keyword. Use the `with` keyword to pass any desired variables.


Examples:

```
on: [push]

jobs:
  ghcr:
    runs-on: ubuntu-latest
    name: "Build and push to GHCR"
    steps:
      - uses: davidslusser/actions_docker_ghcr@v1.0.0
```
<br/>

