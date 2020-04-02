# Cloud Computing - Laboratory 03: Auto scaling an App on Amazon Web Services

Author : Baptiste Hardrick & David Jaquet

## Observation of the Auto Scaling Group behavior

After our Auto Scaling Group created, the group has no instances started. To have 1 instance, we have to stop the Instance created. When we try to stop the instance AWS could not get the instance status as you can see in the screenshot below.

![Bug during the stop of the instance](./assets/BugDuringStopped.png)

However, in our Auto Scaling Group, we can see that we have 1 instance started.

![1 instance is started](./assets/AfterStopAsked.png)

If we return in our instances list, we can see that the instance is well stopped. We can conclude that the problem mentionned before is only a reloading problem.

![Instance terminated](./assets/InstanceStopped.png)

pour instance stopped = existe encore mais inactif; terminated = supprime l'instance