# ANNOUNCEMENT: Temporary Hold on Storage and Compute Requests
As Wynton continues to expand, we are approaching the limits of space, cooling, and power capacity in the Byers Hall server room (BH101). In addition, as we work to move the administration of the cluster to the ARS team, we are currently reprioritizing our workload with the support of Wynton faculty leadership to ensure that we continue to meet our most critical objectives. We understand that this may cause some delays and appreciate your patience and understanding during this period.

Per the email sent to all users on November 25, 2024, there will be a temporary hold on all new storage and compute requests.

# Pricing for Extra Compute

_Example specifications and pricing as of August 2024_

Please note: You cannot be charged for the hardware until it has been received and invoiced. Since lead times can be extensive, please plan as far ahead as you can. 


## Pricing for prioritized "CPU" compute

Cluster compute nodes are purchased by Wynton in modules that have 4 "2U" compute nodes in a single chassis. If partial nodes are requested, contributions will be pooled with other requests towards a full system. **Another option is to pay 180 USD/member.q slot.**


### Configuration: SMC RM224Q 2U Quad-Node Server

This configuration comes with four compute modules, where each node includes:

* CPU/node: 2 × Intel Xeon Gold 5520+ 2.2GHz 28-core processor 

* RAM/node: 256GiB DDR5-4800 ECC (16 × 16 GiB)

* Storage/node: 1 × 1.92TB U.2 NVMe SSD, 1DWPD

Total price for a module with four (4) node: **~37,000 USD** excluding taxes.

As of August 2024, **lead time for compute nodes is approximate three months from order to delivery.** Once the hardware is received, we will schedule time to configure hardware as time allows given priority projects. Unless you are purchasing a four-compute-node module, we will need to wait until we have enough requests to place an order for a whole unit. If we have capacity, we may be able to provision some shares in advance of the billing. 

## Pricing for prioritized Graphics Processing Unit (GPU) processing

<div class="alert alert-info" role="alert" markdown="1">
{{ site.cluster.name }} has {{ site.data.specs.gpu_nodes }} GPU nodes with a total of {{ site.data.specs.gpus }} GPUs available to all users. Among these, {{ site.data.specs.gpu_nodes | minus: site.data.specs.communal_gpu_nodes }} GPU nodes, with a total of {{ site.data.specs.gpus | minus: site.data.specs.communal_gpus }} GPUs, were contributed by different research groups. GPU jobs are limited to 2 hours in length when run on GPUs not contributed by the running user's lab.  In contrast, [contributors are _not_ limited to 2-hour GPU jobs on nodes they contributed](/hpc/scheduler/queues.html). There is also one GPU development node that is available to all users.
</div>

Single GPU cards cannot be purchased - only a full GPU node. However, just like partial compute nodes can be purchased, GPU purchase requests can also be pooled towards a full system. 

There are three common configurations of GPU compute nodes available, which all share the same base setup, and differs only by type of GPU.

### Configuration: Mercury GPU208 2U Server

* CPU: 1 × AMD EPYC 7543P 2.8GHz 32-core processor

* RAM: 512GiB DDR4-3200 (8 × 64GiB)

* Operating-system storage: 1 × 512GB SATA SSD

* Storage: 1 × 960GB U.2 NVMe SSD

Then choose one of:

1. GPU: 4 × Nvidia A40 with 48GB GPU memory (**~25,000 USD**) 

2. GPU: 4 × Nvidia L40 with 48GB GPU memory (**~33,000 USD**)

Note: A100s are no longer available

The prices listed are total prices in USD excluding taxes.  Each price includes the base setup and the corresponding GPU configuration. Warranty is included.  Taxes are calculated and added once hardware is received.

As of October 2023, **lead time for GPUs is approximately 3 months from order to delivery.**  Once the hardware is received, we will schedule time to configure hardware as time allows given priority projects.  


## How to purchase

To purchase compute nodes or GPU nodes, please contact [{{ site.cluster.email_compute }}](mailto:{{ site.cluster.email_compute }}?subject=Request%20to%20purchase%20compute). Please include what you are considering contributing and your UCSF COA [SpeedType] or [chartstring] for billing, along with any questions.

If you are not ready to purchase but have technical questions while you explore options, please contact {{ site.cluster.email_support }}. 

[SpeedType]: https://controller.ucsf.edu/how-to-guides/accounting-reporting/using-ucsf-chart-accounts
[chartstring]: https://controller.ucsf.edu/how-to-guides/accounting-reporting/using-ucsf-chart-accounts
