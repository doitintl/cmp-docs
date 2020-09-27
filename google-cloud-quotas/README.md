# Google Cloud Quotas

Google Compute Engine enforces quotas on resource usage for a variety of reasons; i.e., quotas protect the community of Google Cloud users by preventing unforeseen spikes in usage. As your use of Google Cloud expands over time, your quotas may increase accordingly as not all projects have the same quotas. 

The Cloud Management Platform offers quota monitoring, so when you’re approaching your quotas, we will notify you ahead of time; you can then increase the limits before usage is blocked. In order to start receiving automatic notifications prior to reaching your Google Cloud quotas, your Google Cloud account must be successfully connected.  

To use Google Cloud Quotas, you must verify that your service account was successfully uploaded and granted the appropriate permissions. You can read more on how to configure your Google Cloud accounts at [Connect Your Google Cloud Organization.](../connect-google-cloud-service-account.md)

If successful, you will see:

* Either a Healthy or Partial ****value underneath the Status column in your Configured Accounts widget, and
* Healthy status next to "Core" under the Features widget.

Once that's been set up, you can add the 'Google Cloud Quotas' widget to any of your dashboards within the Cloud Management Platform. You will also start receiving the email notifications as you get close or reach the quotas. 

Navigate to the dashboard you'd like to add the widget to, locate the 'Add Widgets' button and search for 'Google Cloud Quotas', and add the widget to your dashboard. 

To request a quota increase, click on the 'Modify' button, and read the instructions in the Google Cloud [documentation](https://cloud.google.com/compute/quotas).

We are constantly working on monitoring as many quotas as possible. Right now, here is the list of quotas we support.

**Project-based Quotas:**

```text
SNAPSHOTS
NETWORKS
FIREWALLS
IMAGES
STATIC_ADDRESSES
ROUTES
FORWARDING_RULES
TARGET_POOLS
HEALTH_CHECKS
IN_USE_ADDRESSES
TARGET_INSTANCES
TARGET_HTTP_PROXIES
URL_MAPS
BACKEND_SERVICES
INSTANCE_TEMPLATES
TARGET_VPN_GATEWAYS
VPN_TUNNELS
BACKEND_BUCKETS
ROUTERS
TARGET_SSL_PROXIES
TARGET_HTTPS_PROXIES
SSL_CERTIFICATES
SUBNETWORKS
TARGET_TCP_PROXIES
SECURITY_POLICY_RULES
PACKET_MIRRORINGS
NETWORK_ENDPOINT_GROUPS
INTERCONNECTS
GLOBAL_INTERNAL_ADDRESSES
VPN_GATEWAYS
MACHINE_IMAGES
SECURITY_POLICY_CEVAL_RULES
EXTERNAL_VPN_GATEWAYS
PUBLIC_ADVERTISED_PREFIXES
PUBLIC_DELEGATED_PREFIXES
STATIC_BYOIP_ADDRESSES
```

**Region-based Quotas:**

```text
CPUS
DISKS_TOTAL_GB
STATIC_ADDRESSES
IN_USE_ADDRESSES
SSD_TOTAL_GB
LOCAL_SSD_TOTAL_GB
INSTANCE_GROUPS
INSTANCE_GROUP_MANAGERS
INSTANCES
AUTOSCALERS
REGIONAL_AUTOSCALERS
REGIONAL_INSTANCE_GROUP_MANAGERS
PREEMPTIBLE_CPUS
NVIDIA_K80_GPUS
COMMITTED_CPUS
COMMITTED_LOCAL_SSD_TOTAL_GB
COMMITMENTS
NETWORK_ENDPOINT_GROUPS
INTERNAL_ADDRESSES
NVIDIA_P100_GPUS
PREEMPTIBLE_LOCAL_SSD_GB
PREEMPTIBLE_NVIDIA_K80_GPUS
PREEMPTIBLE_NVIDIA_P100_GPUS
NVIDIA_P100_VWS_GPUS
NVIDIA_V100_GPUS
NVIDIA_P4_GPUS
NVIDIA_P4_VWS_GPUS
NODE_GROUPS
NODE_TEMPLATES
PREEMPTIBLE_NVIDIA_V100_GPUS
PREEMPTIBLE_NVIDIA_P4_GPUS
PREEMPTIBLE_NVIDIA_P100_VWS_GPUS
PREEMPTIBLE_NVIDIA_P4_VWS_GPUS
INTERCONNECT_ATTACHMENTS_PER_REGION
INTERCONNECT_ATTACHMENTS_TOTAL_MBPS
RESOURCE_POLICIES
IN_USE_SNAPSHOT_SCHEDULES
NVIDIA_T4_GPUS
NVIDIA_T4_VWS_GPUS
PREEMPTIBLE_NVIDIA_T4_GPUS
PREEMPTIBLE_NVIDIA_T4_VWS_GPUS
IN_USE_BACKUP_SCHEDULES
PUBLIC_DELEGATED_PREFIXES
COMMITTED_NVIDIA_K80_GPUS
COMMITTED_NVIDIA_P100_GPUS
COMMITTED_NVIDIA_P4_GPUS
COMMITTED_NVIDIA_V100_GPUS
COMMITTED_NVIDIA_T4_GPUS
C2_CPUS
N2_CPUS
COMMITTED_N2_CPUS
COMMITTED_C2_CPUS
RESERVATIONS
COMMITTED_LICENSES
N2D_CPUS
COMMITTED_N2D_CPUS
STATIC_BYOIP_ADDRESSES
AFFINITY_GROUPS
NVIDIA_A100_GPUS
PREEMPTIBLE_NVIDIA_A100_GPUS
COMMITTED_NVIDIA_A100_GPUS
A2_CPUS
COMMITTED_A2_CPUS
```

