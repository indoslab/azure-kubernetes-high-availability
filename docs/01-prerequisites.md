# Prerequisites

## Google Cloud Platform

This tutorial leverages the [Google Cloud Platform](https://cloud.google.com/) to streamline provisioning of the compute infrastructure required to bootstrap a Kubernetes cluster from the ground up. [Sign up](https://cloud.google.com/free/) for $300 in free credits.

[Estimated cost](https://cloud.google.com/products/calculator#id=873932bc-0840-4176-b0fa-a8cfd4ca61ae) to run this tutorial: $0.23 per hour ($5.50 per day).

> The compute resources required for this tutorial exceed the Google Cloud Platform free tier.

## Google Cloud Platform SDK

### Install the Google Cloud SDK

Follow the Google Cloud SDK [documentation](https://cloud.google.com/sdk/) to install and configure the `gcloud` command line utility.

Verify the Google Cloud SDK version is 338.0.0 or higher:

```
gcloud version
```

## Running Commands in Parallel with tmux

[tmux](https://github.com/tmux/tmux/wiki) can be used to run commands on multiple compute instances at the same time. Labs in this tutorial may require running the same commands across multiple compute instances, in those cases consider using tmux and splitting a window into multiple panes with synchronize-panes enabled to speed up the provisioning process.

> The use of tmux is optional and not required to complete this tutorial.

![tmux screenshot](images/tmux-screenshot.png)

> Enable synchronize-panes by pressing `ctrl+b` followed by `shift+:`. Next type `set synchronize-panes on` at the prompt. To disable synchronization: `set synchronize-panes off`.

Next: [Part 1 - GCP login and Networking](02-part-01.md)
