---
title: "Microsoft Edge configurations and experimentation"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 10/30/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge configurations and experimentation"
---

# Microsoft Edge configurations and experimentation

This article describes the interaction between Microsoft Edge and the Configuration and Experimentation service. Microsoft Edge communicates with this service to request and receive different kinds of payloads. These payloads can include configurations, feature rollouts and experiments, as well as settings for features and experiments.

> [!NOTE]
> This applies to Microsoft Edge version 77 or later.

## Configurations, Controlled Feature Rollout, and Experiments

Configurations are the payload meant to ensure product health, security, and privacy compliance, and are intended to have the same value for the audience based on platforms and channels. This could be to enable a feature flag for a domain action such as user agent string spoofing or telemetry sampling control. A configuration payload can also be used to disable a feature flag in the event of a bug.

> [!IMPORTANT]
> If the client is air-gapped without Internet access, add the "ecs.skype.com" endpoint to the allowed list to make sure feature flag values can still be received.

### Controlled Feature Rollout

Controlled Feature Rollout (CFR) is a procedure for slowly increasing the size of the user group that receives a feature. By distributing a new feature to a randomly selected subset of the user population, it’s possible to  compare user feedback to an equally sized  subset without the feature to measure the impact of the feature. The kind of information collected is reliability, performance, and any other metrics to ensure the new code is functional and useful, and ready to release to all the users.

### Experiments

Microsoft Edge builds have features and functionality that are still in development or are experimental. Experiments are like CFR, but the size of the user group is much smaller for testing the new concept.  These features are hidden by default until the feature is rolled out or the experiment's finished. Experiment flags are used to enable and disable these features.

## About the service

In all the preceding scenarios, the service delivers the feature flag values to the browser client so they can be applied. Depending on the update, configurations are applied immediately or when the user restarts the browser.  

Organizations can control the interaction with this service using the settings of the [ExperimentationAndConfigurationServiceControl](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#experimentationandconfigurationservicecontrol) policy. You can use this policy to receive configurations only, or get configurations and feature rollouts/experiments.

> [!CAUTION]
> If you disable communications with the service, this will affect Microsoft’s ability to respond to a severe bug in a timely manner.

## See also

- [Microsoft Edge Enterprise landing page](https://www.microsoftedgeinsider.com/enterprise)
- [Microsoft Edge documentation landing page](https://docs.microsoft.com/DeployEdge/)
