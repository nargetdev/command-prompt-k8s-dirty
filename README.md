## purpose

A simple frontend at the command prompt for relaying information about consistency between kubernetes configs i.e. helm charts and the live cluster.

In other words we are providing a simple frontend for the following operation.

> delta between ...
> Abstract Syntax Tree encoded in manifests/helm
> Abstract Syntax Tree queried from live cluster (i.e. using kubectl)

Resulting states could be.

+ IaC ahead ... indicates the infrastructure-as-code config is ahead of the state of cluster (not yet applied)
+ Synchronized
+ Cluster ahead ... indicates the cluster has operations the configs don't have (TODO: perhaps oneday some altruistic soul will create an IDE overlay that indicates *exactly where* that delta lies within the configs (file/linenum)

## Visual Affect

Similar "dirty" warning as accomplished by similar git tools:

➜  lewansoul-lx16a git:(nathan/doxeldrive) ✗ rm dirty_state
➜  lewansoul-lx16a git:(nathan/doxeldrive)
