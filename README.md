# Workspace-level Shared Libraries

Any folder within a cloned repository can contain a shared library. If you have multiple Jenkinsfiles within a single repo this makes it easy to share and extend code between those Jenkinsfiles.

Folder-based libraries are not considered "trusted:" they run in the Groovy sandbox just like typical Pipelines.

```
/* Accessing workspace library */
@Library('script/src/main/groovy') _
```