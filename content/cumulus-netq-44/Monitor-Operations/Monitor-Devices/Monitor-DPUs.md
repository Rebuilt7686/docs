---
title: Monitor DPUs
author: NVIDIA
weight: 850
toc: 3
---

{{<notice note>}}

DPU monitoring is an early access feature. 

{{</notice>}}

With the NetQ UI, you can monitor hardware resources of individual data processing units (DPUs), including CPU utilization, disk usage, and memory utilization.

## View Overall Health of a DPU

For an overview of the current or past health of DPU hardware resources, open the DPU device card. To open a DPU device card:

1. Click {{<img src="/images/netq/devices.svg" alt="empty device card" height="18" width="18">}} (Devices) in the header, then click **Open a device card**.

{{<figure src="/images/netq/open-device-card-42.png" width="250">}}

2. Begin typing the hotsname of the DPU you would like to view. Select it from the suggested matches when it appears.

{{<figure src="/images/netq/add-dpu-auto-suggest-42.png" alt="device card showing 2 DPUs" width="250">}}

3. Click **Add**.

    {{<figure src="/images/netq/dev-medium-dpu-card-42.png" alt="DPU card displaying CPU, memory, and disk utilization statistics" width="200">}}

    This example shows that the *r-netq-bf2-01* DPU has low utilization across CPU, memory, and disks.

### View DPU Attributes

For a quick look at the key attributes of a particular DPU, expand the DPU card using the card size picker.

Attributes are displayed as the default tab on the large DPU card. You can view the static information about the DPU, including its hostname, ASIC vendor and model, CPU information, OS version, and agent version.

{{<figure src="/images/netq/dev-dpu-large-attributes-tab-42.png" alt="large DPU card displaying static DPU information" width="500">}}

To view a larger display of hardware resource utilization, select {{<img src="/images/netq/analytics-bars.svg" alt="large DPU card displaying hardware utilization data" height="18" width="18">}} (Utilization).

{{<figure src="/images/netq/dev-dpu-large-utilization-42.png" width="500">}}
## View Installed Packages

To view the list of installed packages on a particular DPU, expand the card to its largest size using the card size picker.

Installed packages are displayed in a table. You can export the table into other file formats by selecting {{<img src="/images/netq/export.svg" height="18" width="18">}} (Export), and you can filter the table by selecting {{<img src="/images/netq/filter-1.svg" height="18" width="18">}} (Filter).

{{<figure src="/images/netq/dpu-hwresources-l4-installed-packages-42.png" alt="list of packages installed on a DPU" width="1000">}}

## Related Information

- {{<exlink url="https://docs.nvidia.com/doca/sdk/doca-telemetry-service/index.html" text="DOCA Telemetry Service on NVIDIA BlueField DPUs">}}