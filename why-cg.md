| Product Aspect | What is it? | Why? |
| -------------- | ----------- | ---- |
| apk | apk is a package format. Initially designed by Alpine as part of their package management system. | Traditional package managers install or remove packages as a result of requesting install or removal. With apk, install/removal is done as a side effect of modifying system state. Thus apk has reproducible nature - it's declarative. No need for rollback, build will fail if the apk dependency solver is unable to reach installable set of packages. |
| melange | Open source declarative apk builder | You can use a YAML file to define a complete reproducible pipeline to build a package |


## Wolfi vs. Alpine
| Wolfi | Alpine |
| ----- | ------ |
| Does not build its own linux kernel | Does |
| Based on glibc | Based on musl |
| Mitigates performance issues using glibc | Has performance issues |

