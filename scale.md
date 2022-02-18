root@cp1:/home/rattle# kubectl scale --replicas=3 deployment back
deployment.apps/back scaled
root@cp1:/home/rattle# kubectl scale --replicas=3 deployment front
deployment.apps/front scaled

**part of information output**
root@cp1:/home/rattle# kubectl describe nodes
Name:               node1
Roles:              <none>
Non-terminated Pods:          (22 in total)
  Namespace                   Name                                        CPU Requests  CPU Limits  Memory Requests  Memory Limits  Age
  ---------                   ----                                        ------------  ----------  ---------------  -------------  ---
  default                     back-cfbb5c4cf-7vh72                        0 (0%)        0 (0%)      0 (0%)           0 (0%)         96s
  default                     back-cfbb5c4cf-bppd4                        0 (0%)        0 (0%)      0 (0%)           0 (0%)         96s
  default                     back-cfbb5c4cf-pfpkb                        0 (0%)        0 (0%)      0 (0%)           0 (0%)         23m
  default                     front-784597b7cd-684cm                      0 (0%)        0 (0%)      0 (0%)           0 (0%)         3m29s
  default                     front-784597b7cd-9blb4                      0 (0%)        0 (0%)      0 (0%)           0 (0%)         3m29s
  default                     front-784597b7cd-gjwh2                      0 (0%)        0 (0%)      0 (0%)           0 (0%)         19m

