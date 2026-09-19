# Jenkins Pipeline

![Jenkins](https://img.shields.io/badge/Jenkins-D24939?style=flat-square&logo=jenkins&logoColor=white)

A declarative Jenkins pipeline, kept as a minimal reference for pipeline syntax
and stage structure.

## Contents

| File | Purpose |
|---|---|
| `Jenkinsfile` | Declarative pipeline definition |
| `hello.txt` | Build artefact used by the pipeline |
| `Jenkins.pdf` | Accompanying notes |

## Using it

1. Create a new **Pipeline** job in Jenkins.
2. Set *Definition* to **Pipeline script from SCM**.
3. Point it at this repository; Jenkins picks up the `Jenkinsfile` automatically.

```groovy
// the pipeline is declarative, so stages are explicit
pipeline {
    agent any
    stages {
        stage('Build') { /* ... */ }
    }
}
```

Related: [DevOps](https://github.com/cryptic0053/DevOps) ·
[Docker](https://github.com/cryptic0053/Docker)

---

[Anirban Argha](https://github.com/cryptic0053)
