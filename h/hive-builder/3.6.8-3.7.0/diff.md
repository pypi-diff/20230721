# Comparing `tmp/hive_builder-3.6.8.tar.gz` & `tmp/hive_builder-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hive_builder-3.6.8.tar", max compression
+gzip compressed data, was "hive_builder-3.7.0.tar", max compression
```

## Comparing `hive_builder-3.6.8.tar` & `hive_builder-3.7.0.tar`

### file list

```diff
@@ -1,157 +1,159 @@
--rw-r--r--   0        0        0     1074 2023-07-05 01:42:50.382812 hive_builder-3.6.8/LICENSE
--rw-r--r--   0        0        0     1231 2023-07-05 01:42:50.382812 hive_builder-3.6.8/README.md
--rwxr-xr-x   0        0        0      312 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/__init__.py
--rw-r--r--   0        0        0     1031 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/hive-completion.sh
--rw-r--r--   0        0        0    26952 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/hive.py
--rw-r--r--   0        0        0    14020 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/lib/azure_rm_storageshare.py
--rw-r--r--   0        0        0    14954 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/lib/hive_vagrant.py
--rw-r--r--   0        0        0     5832 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/build-images.yml
--rw-r--r--   0        0        0     1943 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/build-infra.yml
--rw-r--r--   0        0        0     1084 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/build-networks.yml
--rw-r--r--   0        0        0     2447 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/build-volumes.yml
--rw-r--r--   0        0        0       81 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/addon/tasks/main.yml
--rw-r--r--   0        0        0       40 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-certificate/files/extfile.cnf
--rw-r--r--   0        0        0     1783 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml
--rw-r--r--   0        0        0      356 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-syslog/tasks/main.yml
--rw-r--r--   0        0        0      946 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2
--rw-r--r--   0        0        0      650 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml
--rw-r--r--   0        0        0      351 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/tasks/main.yml
--rw-r--r--   0        0        0       49 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/vars/main.yml
--rw-r--r--   0        0        0      323 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/tasks/main.yml
--rw-r--r--   0        0        0       49 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/vars/main.yml
--rw-r--r--   0        0        0      409 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/tasks/main.yml
--rw-r--r--   0        0        0       49 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/vars/main.yml
--rw-r--r--   0        0        0      274 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/python-aptk/tasks/main.yml
--rw-r--r--   0        0        0     9564 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/deploy-services.yml
--rw-r--r--   0        0        0     2558 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/group_vars/hosts.yml
--rw-r--r--   0        0        0      129 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/group_vars/mother.yml
--rw-r--r--   0        0        0     1015 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/initialize-services.yml
--rw-r--r--   0        0        0     2430 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/iptables.yml
--rw-r--r--   0        0        0     2479 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/push-image.yml
--rw-r--r--   0        0        0     3107 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/build-aws.yml
--rw-r--r--   0        0        0     3627 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/create_instance.yml
--rw-r--r--   0        0        0     2665 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml
--rw-r--r--   0        0        0      327 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/main.yml
--rw-r--r--   0        0        0      217 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/stop-aws.yml
--rw-r--r--   0        0        0       46 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/templates/aws_cli_config.j2
--rw-r--r--   0        0        0      102 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/templates/aws_cli_credentials.j2
--rw-r--r--   0        0        0      138 2023-07-05 01:42:50.394812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/templates/azure_cli_credentials.j2
--rw-r--r--   0        0        0      138 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/templates/cloudstack.ini.j2
--rw-r--r--   0        0        0     1497 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/aws/vars/main.yml
--rw-r--r--   0        0        0     3273 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/build-azure.yml
--rw-r--r--   0        0        0     3434 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/create_instance.yml
--rw-r--r--   0        0        0     1932 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml
--rw-r--r--   0        0        0      326 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/main.yml
--rw-r--r--   0        0        0      297 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/stop-azure.yml
--rw-r--r--   0        0        0      647 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/azure/vars/main.yml
--rw-r--r--   0        0        0      589 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/tasks/main.yml
--rw-r--r--   0        0        0      179 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/templates/backup.service
--rw-r--r--   0        0        0      126 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/templates/backup.timer
--rw-r--r--   0        0        0     5210 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh
--rw-r--r--   0        0        0       85 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/base/files/NetworkManager-wait-online.service.d/override.conf
--rw-r--r--   0        0        0     1210 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml
--rw-r--r--   0        0        0     1796 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/growfs.yml
--rw-r--r--   0        0        0     6801 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/main.yml
--rw-r--r--   0        0        0       77 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/ca/files/extfile.cnf
--rw-r--r--   0        0        0     1290 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/ca/tasks/main.yml
--rw-r--r--   0        0        0      268 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/ca/vars/main.yml
--rw-r--r--   0        0        0     4726 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker/tasks/main.yml
--rw-r--r--   0        0        0      321 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker/templates/daemon.json.j2
--rw-r--r--   0        0        0      331 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker/templates/override.conf
--rw-r--r--   0        0        0     2301 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/tasks/main.yml
--rw-r--r--   0        0        0     1770 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dcp
--rw-r--r--   0        0        0     1467 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dexec
--rw-r--r--   0        0        0      678 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dsh
--rw-r--r--   0        0        0      170 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/vars/main.yml
--rw-r--r--   0        0        0     1032 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml
--rw-r--r--   0        0        0      233 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client-proxy/templates/config.json.j2
--rw-r--r--   0        0        0      147 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/docker-compose/tasks/main.yml
--rw-r--r--   0        0        0      229 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/files/drbd-resource@.service
--rw-r--r--   0        0        0      309 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/files/waitdevice
--rw-r--r--   0        0        0     3060 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/tasks/main.yml
--rw-r--r--   0        0        0     3381 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/tasks/vg.yml
--rw-r--r--   0        0        0      442 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/vars/main.yml
--rw-r--r--   0        0        0     5426 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml
--rw-r--r--   0        0        0     1568 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/templates/volume.res
--rw-r--r--   0        0        0      421 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/vars/main.yml
--rw-r--r--   0        0        0    27684 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py
--rw-r--r--   0        0        0     1411 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml
--rw-r--r--   0        0        0      309 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/templates/follow-swarm-service.service
--rw-r--r--   0        0        0     2850 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml
--rw-r--r--   0        0        0     3021 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml
--rw-r--r--   0        0        0     3289 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml
--rw-r--r--   0        0        0      314 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/main.yml
--rw-r--r--   0        0        0      396 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/stop-gcp.yml
--rw-r--r--   0        0        0      741 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/vars/main.yml
--rw-r--r--   0        0        0      338 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/hostsfile/tasks/main.yml
--rw-r--r--   0        0        0     1403 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/internal-network/tasks/main.yml
--rw-r--r--   0        0        0      625 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/iptables/tasks/main.yml
--rw-r--r--   0        0        0     4319 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/tasks/main.yml
--rw-r--r--   0        0        0     3345 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2
--rw-r--r--   0        0        0      171 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/vars/main.yml
--rw-r--r--   0        0        0      118 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/handlers/main.yml
--rw-r--r--   0        0        0      875 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml
--rw-r--r--   0        0        0     1017 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2
--rw-r--r--   0        0        0     2436 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml
--rw-r--r--   0        0        0     2001 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml
--rw-r--r--   0        0        0     2528 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml
--rw-r--r--   0        0        0      531 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/ntp-client/tasks/main.yml
--rw-r--r--   0        0        0     2650 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/pip-venv/tasks/main.yml
--rw-r--r--   0        0        0      403 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/prepared/tasks/main.yml
--rw-r--r--   0        0        0      665 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/prepared/tasks/setup.yml
--rw-r--r--   0        0        0       79 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/prepared/vars/main.yml
--rw-r--r--   0        0        0      394 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/reboot/handlers/main.yml
--rw-r--r--   0        0        0     1712 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/registry/tasks/main.yml
--rw-r--r--   0        0        0       57 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/registry/templates/daemon.json.j2
--rw-r--r--   0        0        0      985 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/registry/templates/registry.yml.j2
--rw-r--r--   0        0        0      118 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/handlers/main.yml
--rw-r--r--   0        0        0     1338 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml
--rw-r--r--   0        0        0     3184 2023-07-05 01:42:50.398812 hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/templates/services.conf
--rw-r--r--   0        0        0      788 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/service-backup/tasks/main.yml
--rw-r--r--   0        0        0     5337 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2
--rw-r--r--   0        0        0     1148 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml
--rw-r--r--   0        0        0     7628 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/swarm/tasks/main.yml
--rw-r--r--   0        0        0      220 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/handlers/main.yml
--rw-r--r--   0        0        0     2912 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml
--rw-r--r--   0        0        0      188 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/templates/extfile.cnf
--rw-r--r--   0        0        0      508 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/vars/main.yml
--rw-r--r--   0        0        0      433 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/users/tasks/known-hosts.yml
--rw-r--r--   0        0        0     1157 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/users/tasks/main.yml
--rw-r--r--   0        0        0       40 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/users/templates/sudoer.j2
--rw-r--r--   0        0        0     3160 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/files/Vagrantfile
--rw-r--r--   0        0        0     1078 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/files/growfs.sh
--rw-r--r--   0        0        0     2413 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/tasks/main.yml
--rw-r--r--   0        0        0     1116 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2
--rw-r--r--   0        0        0     3414 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml
--rw-r--r--   0        0        0     8115 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml
--rw-r--r--   0        0        0     1601 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml
--rw-r--r--   0        0        0     2337 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-server.xml
--rw-r--r--   0        0        0     4694 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/tasks/main.yml
--rw-r--r--   0        0        0     2638 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2
--rw-r--r--   0        0        0      269 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/vars/main.yml
--rw-r--r--   0        0        0      144 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/ausearch.conf
--rw-r--r--   0        0        0    14795 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py
--rw-r--r--   0        0        0     1337 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py
--rw-r--r--   0        0        0      269 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/drbd-resource.conf
--rw-r--r--   0        0        0     6520 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/hive.te
--rw-r--r--   0        0        0     4960 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn
--rw-r--r--   0        0        0      115 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/service_discovery_blacklist
--rw-r--r--   0        0        0       62 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/sudoers.zabbix
--rw-r--r--   0        0        0      360 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/userparameter_systemd_services.conf
--rw-r--r--   0        0        0      739 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh
--rw-r--r--   0        0        0      461 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_restart_check.sh
--rw-r--r--   0        0        0      389 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/handlers/main.yml
--rw-r--r--   0        0        0     6203 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml
--rw-r--r--   0        0        0     1397 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2
--rw-r--r--   0        0        0      345 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/docker-volume.j2
--rw-r--r--   0        0        0      354 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.service
--rw-r--r--   0        0        0      196 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.timer
--rw-r--r--   0        0        0    10611 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2
--rw-r--r--   0        0        0      681 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml
--rw-r--r--   0        0        0     2482 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/playbooks/setup-hosts.yml
--rw-r--r--   0        0        0    20038 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/plugins/hive_inventory.py
--rw-r--r--   0        0        0    14761 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/plugins/hive_services.py
--rw-r--r--   0        0        0      235 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/requirements.yml
--rw-r--r--   0        0        0    11579 2023-07-05 01:42:50.402812 hive_builder-3.6.8/hive_builder/variables_metainf.yml
--rw-r--r--   0        0        0      633 2023-07-05 01:42:50.402812 hive_builder-3.6.8/pyproject.toml
--rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 hive_builder-3.6.8/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-21 09:04:32.057621 hive_builder-3.7.0/LICENSE
+-rw-r--r--   0        0        0     1231 2023-07-21 09:04:32.057621 hive_builder-3.7.0/README.md
+-rwxr-xr-x   0        0        0      312 2023-07-21 09:04:32.069622 hive_builder-3.7.0/hive_builder/__init__.py
+-rw-r--r--   0        0        0     1031 2023-07-21 09:04:32.069622 hive_builder-3.7.0/hive_builder/hive-completion.sh
+-rw-r--r--   0        0        0    27108 2023-07-21 09:04:32.069622 hive_builder-3.7.0/hive_builder/hive.py
+-rw-r--r--   0        0        0    14020 2023-07-21 09:04:32.069622 hive_builder-3.7.0/hive_builder/lib/azure_rm_storageshare.py
+-rw-r--r--   0        0        0    14954 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/lib/hive_vagrant.py
+-rw-r--r--   0        0        0     5893 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/build-images.yml
+-rw-r--r--   0        0        0     1943 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/build-infra.yml
+-rw-r--r--   0        0        0     1084 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/build-networks.yml
+-rw-r--r--   0        0        0     2447 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/build-volumes.yml
+-rw-r--r--   0        0        0       81 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/addon/tasks/main.yml
+-rw-r--r--   0        0        0       40 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-certificate/files/extfile.cnf
+-rw-r--r--   0        0        0     1783 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml
+-rw-r--r--   0        0        0      356 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-syslog/tasks/main.yml
+-rw-r--r--   0        0        0      946 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2
+-rw-r--r--   0        0        0      650 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml
+-rw-r--r--   0        0        0      587 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-trust-ca-alpine/vars/main.yml
+-rw-r--r--   0        0        0      466 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-trust-ca-centos/vars/main.yml
+-rw-r--r--   0        0        0      534 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/tasks/main.yml
+-rw-r--r--   0        0        0       49 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-trust-ca-ubuntu/vars/main.yml
+-rw-r--r--   0        0        0      935 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/python-aptk/tasks/main.yml
+-rw-r--r--   0        0        0     9794 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/deploy-services.yml
+-rw-r--r--   0        0        0     2162 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/group_vars/hosts.yml
+-rw-r--r--   0        0        0      129 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/group_vars/mother.yml
+-rw-r--r--   0        0        0     1015 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/initialize-services.yml
+-rw-r--r--   0        0        0     2430 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/iptables.yml
+-rw-r--r--   0        0        0     2479 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/push-image.yml
+-rw-r--r--   0        0        0     3107 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/tasks/build-aws.yml
+-rw-r--r--   0        0        0     3744 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/tasks/create_instance.yml
+-rw-r--r--   0        0        0     2665 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml
+-rw-r--r--   0        0        0      327 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/tasks/main.yml
+-rw-r--r--   0        0        0      217 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/tasks/stop-aws.yml
+-rw-r--r--   0        0        0       46 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/templates/aws_cli_config.j2
+-rw-r--r--   0        0        0      102 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/templates/aws_cli_credentials.j2
+-rw-r--r--   0        0        0      138 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/templates/azure_cli_credentials.j2
+-rw-r--r--   0        0        0      138 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/templates/cloudstack.ini.j2
+-rw-r--r--   0        0        0     1497 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/aws/vars/main.yml
+-rw-r--r--   0        0        0     3273 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/azure/tasks/build-azure.yml
+-rw-r--r--   0        0        0     3551 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/azure/tasks/create_instance.yml
+-rw-r--r--   0        0        0     1932 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml
+-rw-r--r--   0        0        0      326 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/azure/tasks/main.yml
+-rw-r--r--   0        0        0      297 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/azure/tasks/stop-azure.yml
+-rw-r--r--   0        0        0      647 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/azure/vars/main.yml
+-rw-r--r--   0        0        0      589 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/backup-tools/tasks/main.yml
+-rw-r--r--   0        0        0      179 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/backup-tools/templates/backup.service
+-rw-r--r--   0        0        0      126 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/backup-tools/templates/backup.timer
+-rw-r--r--   0        0        0     5210 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh
+-rw-r--r--   0        0        0       85 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/base/files/NetworkManager-wait-online.service.d/override.conf
+-rw-r--r--   0        0        0     1255 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml
+-rw-r--r--   0        0        0     1796 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/base/tasks/growfs.yml
+-rw-r--r--   0        0        0     6944 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/base/tasks/main.yml
+-rw-r--r--   0        0        0      567 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/base/tasks/pip_index_url.yml
+-rw-r--r--   0        0        0     1407 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/base/tasks/setup_proxy_env.yml
+-rw-r--r--   0        0        0       77 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/ca/files/extfile.cnf
+-rw-r--r--   0        0        0     1290 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/ca/tasks/main.yml
+-rw-r--r--   0        0        0      268 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/ca/vars/main.yml
+-rw-r--r--   0        0        0     5554 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker/tasks/main.yml
+-rw-r--r--   0        0        0      425 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker/templates/daemon.json.j2
+-rw-r--r--   0        0        0      331 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker/templates/override.conf
+-rw-r--r--   0        0        0     2301 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/tasks/main.yml
+-rw-r--r--   0        0        0     1770 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/templates/dcp
+-rw-r--r--   0        0        0     1467 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/templates/dexec
+-rw-r--r--   0        0        0      678 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/templates/dsh
+-rw-r--r--   0        0        0      170 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/vars/main.yml
+-rw-r--r--   0        0        0     1032 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml
+-rw-r--r--   0        0        0      233 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client-proxy/templates/config.json.j2
+-rw-r--r--   0        0        0      147 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/docker-compose/tasks/main.yml
+-rw-r--r--   0        0        0      229 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/drbd/files/drbd-resource@.service
+-rw-r--r--   0        0        0      309 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/drbd/files/waitdevice
+-rw-r--r--   0        0        0     3060 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/drbd/tasks/main.yml
+-rw-r--r--   0        0        0     3381 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/drbd/tasks/vg.yml
+-rw-r--r--   0        0        0      442 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/drbd/vars/main.yml
+-rw-r--r--   0        0        0     5426 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml
+-rw-r--r--   0        0        0     1568 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/drbd-resource/templates/volume.res
+-rw-r--r--   0        0        0      421 2023-07-21 09:04:32.073622 hive_builder-3.7.0/hive_builder/playbooks/roles/drbd-resource/vars/main.yml
+-rw-r--r--   0        0        0    27684 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py
+-rw-r--r--   0        0        0     1411 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml
+-rw-r--r--   0        0        0      309 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/follow-swarm-service/templates/follow-swarm-service.service
+-rw-r--r--   0        0        0     2850 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml
+-rw-r--r--   0        0        0     3138 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml
+-rw-r--r--   0        0        0     3289 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml
+-rw-r--r--   0        0        0      314 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/tasks/main.yml
+-rw-r--r--   0        0        0      396 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/tasks/stop-gcp.yml
+-rw-r--r--   0        0        0      741 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/vars/main.yml
+-rw-r--r--   0        0        0      338 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/hostsfile/tasks/main.yml
+-rw-r--r--   0        0        0     1403 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/internal-network/tasks/main.yml
+-rw-r--r--   0        0        0      625 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/iptables/tasks/main.yml
+-rw-r--r--   0        0        0     4436 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/kickstart/tasks/main.yml
+-rw-r--r--   0        0        0     3345 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2
+-rw-r--r--   0        0        0      171 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/kickstart/vars/main.yml
+-rw-r--r--   0        0        0      118 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/monitor-service-log/handlers/main.yml
+-rw-r--r--   0        0        0      875 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml
+-rw-r--r--   0        0        0     1017 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2
+-rw-r--r--   0        0        0     2436 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml
+-rw-r--r--   0        0        0     2001 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml
+-rw-r--r--   0        0        0     2528 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml
+-rw-r--r--   0        0        0      531 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/ntp-client/tasks/main.yml
+-rw-r--r--   0        0        0     2407 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/pip-venv/tasks/main.yml
+-rw-r--r--   0        0        0      403 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/prepared/tasks/main.yml
+-rw-r--r--   0        0        0      782 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/prepared/tasks/setup.yml
+-rw-r--r--   0        0        0       79 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/prepared/vars/main.yml
+-rw-r--r--   0        0        0      394 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/reboot/handlers/main.yml
+-rw-r--r--   0        0        0     1712 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/registry/tasks/main.yml
+-rw-r--r--   0        0        0       57 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/registry/templates/daemon.json.j2
+-rw-r--r--   0        0        0      985 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/registry/templates/registry.yml.j2
+-rw-r--r--   0        0        0      118 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/rsyslogd/handlers/main.yml
+-rw-r--r--   0        0        0     1338 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml
+-rw-r--r--   0        0        0     3184 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/rsyslogd/templates/services.conf
+-rw-r--r--   0        0        0      788 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/service-backup/tasks/main.yml
+-rw-r--r--   0        0        0     5337 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2
+-rw-r--r--   0        0        0     1148 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml
+-rw-r--r--   0        0        0     7628 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/swarm/tasks/main.yml
+-rw-r--r--   0        0        0      220 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/tls-certificate/handlers/main.yml
+-rw-r--r--   0        0        0     2912 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml
+-rw-r--r--   0        0        0      188 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/tls-certificate/templates/extfile.cnf
+-rw-r--r--   0        0        0      508 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/tls-certificate/vars/main.yml
+-rw-r--r--   0        0        0      433 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/users/tasks/known-hosts.yml
+-rw-r--r--   0        0        0     1157 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/users/tasks/main.yml
+-rw-r--r--   0        0        0       40 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/users/templates/sudoer.j2
+-rw-r--r--   0        0        0     3160 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/vagrant/files/Vagrantfile
+-rw-r--r--   0        0        0     1078 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/vagrant/files/growfs.sh
+-rw-r--r--   0        0        0     2673 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/vagrant/tasks/main.yml
+-rw-r--r--   0        0        0     1116 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2
+-rw-r--r--   0        0        0     3414 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml
+-rw-r--r--   0        0        0     8115 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml
+-rw-r--r--   0        0        0     1601 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml
+-rw-r--r--   0        0        0     2337 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/files/hive-server.xml
+-rw-r--r--   0        0        0     4694 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/tasks/main.yml
+-rw-r--r--   0        0        0     2638 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2
+-rw-r--r--   0        0        0      269 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/vars/main.yml
+-rw-r--r--   0        0        0      144 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/ausearch.conf
+-rw-r--r--   0        0        0    14795 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py
+-rw-r--r--   0        0        0     1337 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py
+-rw-r--r--   0        0        0      269 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/drbd-resource.conf
+-rw-r--r--   0        0        0     6520 2023-07-21 09:04:32.077623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/hive.te
+-rw-r--r--   0        0        0     4960 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn
+-rw-r--r--   0        0        0      115 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/service_discovery_blacklist
+-rw-r--r--   0        0        0       62 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/sudoers.zabbix
+-rw-r--r--   0        0        0      360 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/userparameter_systemd_services.conf
+-rw-r--r--   0        0        0      739 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh
+-rw-r--r--   0        0        0      461 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_restart_check.sh
+-rw-r--r--   0        0        0      389 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/handlers/main.yml
+-rw-r--r--   0        0        0     6006 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml
+-rw-r--r--   0        0        0     1397 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2
+-rw-r--r--   0        0        0      345 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/templates/docker-volume.j2
+-rw-r--r--   0        0        0      354 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.service
+-rw-r--r--   0        0        0      196 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix-agent-cache-builder.timer
+-rw-r--r--   0        0        0    10611 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2
+-rw-r--r--   0        0        0      681 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml
+-rw-r--r--   0        0        0     2482 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/playbooks/setup-hosts.yml
+-rw-r--r--   0        0        0    20038 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/plugins/hive_inventory.py
+-rw-r--r--   0        0        0    14761 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/plugins/hive_services.py
+-rw-r--r--   0        0        0      259 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/requirements.yml
+-rw-r--r--   0        0        0    12245 2023-07-21 09:04:32.081623 hive_builder-3.7.0/hive_builder/variables_metainf.yml
+-rw-r--r--   0        0        0      633 2023-07-21 09:04:32.081623 hive_builder-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2150 1970-01-01 00:00:00.000000 hive_builder-3.7.0/PKG-INFO
```

### Comparing `hive_builder-3.6.8/LICENSE` & `hive_builder-3.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/README.md` & `hive_builder-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/hive-completion.sh` & `hive_builder-3.7.0/hive_builder/hive-completion.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/hive.py` & `hive_builder-3.7.0/hive_builder/hive.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,20 +413,23 @@
     ssh_config_path = context.vars['context_dir'] + '/ssh_config'
     grep_proc = subprocess.run(['grep', '^Host ', ssh_config_path], stdout=subprocess.PIPE)
     if grep_proc.returncode == 1:
       raise Error(f'no Host entry in {ssh_config_path}')
     if grep_proc.returncode != 0:
       raise Error(f'fail to read ssh_config {ssh_config_path} error, you may never done build-infra: {grep_proc.stderr}')
     ssh_tunnel_procs = []
+    http_proxy = context.vars.get('http_proxy')
     for host_name in map(lambda x: x.decode(encoding='utf-8').split(' ')[1], grep_proc.stdout.splitlines()):
       socket_path = f'{context.vars["temp_dir"]}/docker.sock@{host_name}'
       if pathlib.Path(socket_path).is_socket():
         raise Error(f'fail to create socket {socket_path}, another hive process may doing build-images/deploy-services' +
                     ' or the file has been left because previus hive process aborted suddenly')
       args = ['ssh', '-N', '-F', ssh_config_path, '-L', socket_path + ':/var/run/docker.sock', host_name]
+      if http_proxy is not None:
+        args += ['-R', context.vars['http_proxy_port'] + ':' + http_proxy]
       ssh_tunnel_procs.append((socket_path, subprocess.Popen(args)))
     try:
       super().do_one(context)
     finally:
       for socket_path, ssh_tunnel_proc in ssh_tunnel_procs:
         ssh_tunnel_proc.send_signal(signal.SIGTERM)
         while ssh_tunnel_proc.poll() is None:
```

### Comparing `hive_builder-3.6.8/hive_builder/lib/azure_rm_storageshare.py` & `hive_builder-3.7.0/hive_builder/lib/azure_rm_storageshare.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/lib/hive_vagrant.py` & `hive_builder-3.7.0/hive_builder/lib/hive_vagrant.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/build-images.yml` & `hive_builder-3.7.0/hive_builder/playbooks/build-images.yml`

 * *Files 6% similar despite different names*

```diff
@@ -45,14 +45,17 @@
       hive_safe_proxy_settings:
         HTTP_PROXY: "{{ hostvars[hive_safe_repository_server].ansible_env.HTTP_PROXY | default('') }}"
         http_proxy: "{{ hostvars[hive_safe_repository_server].ansible_env.http_proxy | default('') }}"
         HTTPS_PROXY: "{{ hostvars[hive_safe_repository_server].ansible_env.HTTPS_PROXY | default('') }}"
         https_proxy: "{{ hostvars[hive_safe_repository_server].ansible_env.https_proxy | default('') }}"
         NO_PROXY: "{{ hostvars[hive_safe_repository_server].ansible_env.NO_PROXY | default('') }}"
         no_proxy: "{{ hostvars[hive_safe_repository_server].ansible_env.no_proxy | default('') }}"
+        PIP_CERT: "{{ '/etc/cacert_pip.pem' if hive_http_proxy is defined else omit }}"
+        PIP_INDEX_URL: "{{ hostvars[hive_safe_repository_server].ansible_env.PIP_INDEX_URL | default('') }}"
+        PIP_TRUSTED_HOST: "{{ hostvars[hive_safe_repository_server].ansible_env.PIP_TRUSTED_HOST | default('') }}"
   - name: create container
     delegate_to: "{{ hive_safe_repository_server }}"
     docker_container:
       image: >-
         {%- if hive_from in tag_mapping_json.keys() -%}
           {{ tag_mapping_json[hive_from] }}
         {%- else -%}
@@ -64,35 +67,37 @@
       env: "{{(hive_env | default({})) | combine(hive_safe_proxy_settings) }}"
       privileged: "{{ hive_privileged | default(omit) }}"
       entrypoint: "{%if hive_standalone | default(False) %}{{omit}}{%else%}[]{%endif%}"
       working_dir: "{{ hive_working_dir | default(omit) }}"
       command: "{%if hive_standalone | default(False) %}{{omit}}{%else%}{{ hive_safe_sleep_command }}{%endif%}"
       stop_signal: "{{ hive_stop_signal | default(omit) }}"
       user: "{{ hive_user | default(omit) }}"
+      command_handling: correct
       state: present
     when: hive_stage not in (hive_pull_on | default([]))
   - name: start container
     delegate_to: "{{ hive_safe_repository_server }}"
     docker_container:
       image: >-
         {%- if hive_from in tag_mapping_json.keys() -%}
           {{ tag_mapping_json[hive_from] }}
         {%- else -%}
           {{ hive_from }}
         {%- endif -%}
       exposed_ports: "{{ hive_expose | default(omit) }}"
       name: "build_{{ inventory_hostname }}"
       hostname: "{{ inventory_hostname }}"
-      env: "{%if lookup('env', 'HTTP_PROXY') | length > 0 %}{{(hive_env | default({}))|combine({'HTTP_PROXY':lookup('env', 'HTTP_PROXY'),'http_proxy':lookup('env', 'HTTP_PROXY'),'HTTPS_PROXY':lookup('env', 'HTTPS_PROXY'),'https_proxy':lookup('env', 'HTTPS_PROXY'),'NO_PROXY':lookup('env', 'NO_PROXY'),'no_proxy':lookup('env', 'NO_PROXY')})}}{% else %}{{ hive_env | default(omit) }}{% endif %}"
+      env: "{{(hive_env | default({})) | combine(hive_safe_proxy_settings) }}"
       privileged: "{{ hive_privileged | default(omit) }}"
       entrypoint: "{%if hive_standalone | default(False) %}{{omit}}{%else%}[]{%endif%}"
       working_dir: "{{ hive_working_dir | default(omit) }}"
       command: "{%if hive_standalone | default(False) %}{{omit}}{%else%}{{ hive_safe_sleep_command }}{%endif%}"
       stop_signal: "{{ hive_stop_signal | default(omit) }}"
       user: "{{ hive_user | default(omit) }}"
+      command_handling: correct
     changed_when: False
     when: hive_stage not in (hive_pull_on | default([]))
   - name: apply role
     include_role:
       name: "{{ hive_safe_role }}"
     vars:
       ansible_host: "build_{{ inventory_hostname }}"
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/build-infra.yml` & `hive_builder-3.7.0/hive_builder/playbooks/build-infra.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/build-networks.yml` & `hive_builder-3.7.0/hive_builder/playbooks/build-networks.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/build-volumes.yml` & `hive_builder-3.7.0/hive_builder/playbooks/build-volumes.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-certificate/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2` & `hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-syslog/templates/transfer.conf.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/builtin_roles/hive-trust-ca/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/deploy-services.yml` & `hive_builder-3.7.0/hive_builder/playbooks/deploy-services.yml`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,17 @@
     hive_safe_proxy_setting:
       HTTP_PROXY: "{{ ansible_env.HTTP_PROXY | default('') }}"
       http_proxy: "{{ ansible_env.http_proxy  | default('') }}"
       HTTPS_PROXY: "{{ ansible_env.HTTPS_PROXY | default('') }}"
       https_proxy: "{{ ansible_env.https_proxy  | default('') }}"
       NO_PROXY: "{{ ansible_env.NO_PROXY | default('') }}"
       no_proxy: "{{ ansible_env.no_proxy  | default('') }}"
+      PIP_CERT: "{{ '/etc/cacert_pip.pem' if hive_http_proxy is defined else omit }}"
+      PIP_INDEX_URL: "{{ ansible_env.PIP_INDEX_URL | default('') }}"
+      PIP_TRUSTED_HOST: "{{ ansible_env.PIP_TRUSTED_HOST | default('') }}"
 
   tasks:
   - name: get containers for the serivce
     shell: |
       docker service ps --format '{% raw %}{"name": "{{.Name}}.{{.ID}}", "node": "{{.Node}}{% endraw %}.{{ hive_name }}"}' --filter desired-state=running --no-trunc {{ item }}
     changed_when: False
     check_mode: False
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/group_vars/hosts.yml` & `hive_builder-3.7.0/hive_builder/playbooks/group_vars/hosts.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,10 @@
 ---
 hive_safe_email: "{{ hive_email | default('hive@example.com') }}"
 hive_safe_docker_login_user: "{{ hive_docker_login_user | default('hive') }}"
-hive_http_proxy: "lookup('env', 'HTTP_PROXY')"
-hive_https_proxy: "lookup('env', 'HTTPS_PROXY')"
-hive_no_proxy: "lookup('env', 'NO_PROXY')"
-hive_tmp_proxy_env_block: |
-  HTTP_PROXY={{ hive_http_proxy }}
-  HTTPS_PROXY={{ hive_https_proxy }}
-  NO_PROXY={{ hive_no_proxy }}
-hive_proxy_env_block: "{%if lookup('env', 'HTTP_PROXY') | length > 0 %}{{hive_tmp_proxy_env_block}}{%else%}{{omit}}{%endif%}"
 hive_registry: "{{ hive_registry_fqdn }}:{{ hive_registry_port | default(5000) }}"
 hive_safe_private_key_path:  "{{ hive_private_key_path | default(hive_context_dir + '/id_rsa') }}"
 hive_safe_public_key_path:  "{{ hive_public_key_path | default(hive_safe_private_key_path + '.pub') }}"
 hive_published_ports_tcp: "{{ groups['services'] | map('extract', hostvars, 'hive_ports') | select('defined') | flatten | selectattr('protocol', 'eq', 'tcp') | selectattr('published_port', 'defined') | selectattr('published_port', 'lt', 10000) | map(attribute='published_port') | map('string') | list }}"
 hive_published_ports_udp: "{{ groups['services'] | map('extract', hostvars, 'hive_ports') | select('defined') | flatten | selectattr('protocol', 'eq', 'udp') | selectattr('published_port', 'defined') | selectattr('published_port', 'lt', 10000) | map(attribute='published_port') | map('string') |  list }}"
 # 2019/12/30  username "admin" cause error for azure:
 #    Error creating or updating virtual machine hive0 - Azure Error: InvalidParameter
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/initialize-services.yml` & `hive_builder-3.7.0/hive_builder/playbooks/initialize-services.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/iptables.yml` & `hive_builder-3.7.0/hive_builder/playbooks/iptables.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/push-image.yml` & `hive_builder-3.7.0/hive_builder/playbooks/push-image.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/build-aws.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/aws/tasks/build-aws.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/create_instance.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/aws/tasks/create_instance.yml`

 * *Files 2% similar despite different names*

```diff
@@ -80,8 +80,9 @@
         UserKnownHostsFile {{ hive_context_dir }}/known_hosts
         StrictHostKeyChecking yes
         User {{ hive_safe_admin }}
         PasswordAuthentication no
         IdentityFile {{ hive_safe_private_key_path }}
         IdentitiesOnly yes
         LogLevel FATAL
+      {% if hive_http_proxy is defined %}  RemoteForward {{ hive_http_proxy_port }} {{ hive_http_proxy }}{% endif %}
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/aws/tasks/destroy-aws.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/aws/vars/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/aws/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/build-azure.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/azure/tasks/build-azure.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/create_instance.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/azure/tasks/create_instance.yml`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,15 @@
         UserKnownHostsFile {{ hive_context_dir }}/known_hosts
         StrictHostKeyChecking yes
         User {{ hive_safe_admin }}
         PasswordAuthentication no
         IdentityFile {{ hive_safe_private_key_path }}
         IdentitiesOnly yes
         LogLevel FATAL
+      {% if hive_http_proxy is defined %}  RemoteForward {{ hive_http_proxy_port }} {{ hive_http_proxy }}{% endif %}
 
 - name: Create default network inteface card
   azure_rm_networkinterface:
     resource_group: "{{ hive_safe_azure_resourcegroup }}"
     name: "{{hive_safe_name}}-primary"
     virtual_network: "{{ hive_safe_vpc_name }}"
     subnet: "{{ hostvars[azure_host].hive_subnet }}"
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/azure/tasks/destroy-azure.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/azure/vars/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/azure/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/backup-tools/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh` & `hive_builder-3.7.0/hive_builder/playbooks/roles/backup-tools/templates/hive-backup.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/base/tasks/fixed-yum-url.yml`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,16 @@
   - CentOS-Linux-AppStream.repo
   - CentOS-Linux-BaseOS.repo
   - CentOS-Linux-Extras.repo
   # stream 8
   - CentOS-Stream-AppStream.repo
   - CentOS-Stream-Base.repo
   - CentOS-Stream-Extras.repo
+  # almalinux
+  - almalinux.repo
 - name: Disable yum-fastestmirror
   lineinfile: >
     dest="/etc/yum/pluginconf.d/fastestmirror.conf"
     line="enabled=0"
     state=present
     regexp="^#?enabled="
     insertafter=EOF
@@ -30,10 +32,10 @@
     path: "/etc/yum.repos.d/{{ item }}"
     regexp: "^#?mirrorlist=(.*)$"
     replace: "#mirrorlist=\\1"
   loop: "{{ repo_files.results | selectattr('stat.exists', 'eq', True) | map(attribute='item') | list }}"
 - name: fix yum download site - set baseurl
   replace:
     path: "/etc/yum.repos.d/{{ item }}"
-    regexp: "^#?baseurl=.*/(centos|\\$contentdir)/(.*)$"
+    regexp: "^#? *baseurl=.*/(centos|\\$contentdir|almalinux)/(.*)$"
     replace: "baseurl={{ hive_yum_url }}/\\2"
   loop: "{{ repo_files.results | selectattr('stat.exists', 'eq', True) | map(attribute='item') | list }}"
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/growfs.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/base/tasks/growfs.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/base/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/base/tasks/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 ---
 # common utiility packages.
 - import_tasks: fixed-yum-url.yml
   when: ansible_distribution != 'Amazon' and hive_yum_url is defined and hive_yum_url != omit
 - import_tasks: growfs.yml
   when: hive_provider == 'azure' and hive_disk_size is defined
+- import_tasks: setup_proxy_env.yml
+  when: hive_http_proxy is defined
+- import_tasks: pip_index_url.yml
+  when: hive_pip_index_url is defined
 - name: install nfs utils
   yum: name=nfs-utils state=present
   when: groups['nfs_volumes'] | length > 0
 - name: activate nfs service
   service: name=nfs enabled=yes state=started
   when: groups['nfs_volumes'] | length > 0 and ansible_distribution == 'Amazon'
 - name: make yum do not update kernel* package
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/ca/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/ca/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/docker/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/docker/tasks/main.yml`

 * *Files 8% similar despite different names*

```diff
@@ -78,14 +78,26 @@
 - import_tasks: iptables.yml
   vars:
     hive_safe_iptables_name: docker_swarm_udp
     hive_safe_iptables_dports:
       - 7946
       - 4789
     hive_safe_iptables_protocol: udp
+- import_tasks: iptables.yml
+  vars:
+    hive_safe_iptables_name: http_proxy
+    hive_safe_iptables_dports:
+      - "{{ hive_http_proxy_port }}"
+    hive_safe_iptables_protocol: tcp
+    hive_safe_iptables_sources: "{{ (groups['servers'] | intersect(groups[hive_stage]) | map('extract', hostvars, 'hive_private_ip') | list) +
+      [hive_internal_cidr | ipaddr((hive_internal_cidr | ipaddr('size')) / 8 * 4) | ipaddr('address') + '/' +
+      (((hive_internal_cidr | ipaddr('prefix')) + 3) | string) if hive_internal_cidr is defined else '172.20.0.0/16'] +
+      [hive_internal_cidr | ipaddr(((hive_internal_cidr | ipaddr('size')) / 8 * 5) + 1) | ipaddr('address') + '/' +
+      (((hive_internal_cidr | ipaddr('prefix')) + 3) | string) if hive_internal_cidr is defined else '172.17.0.0/16'] }}"
+  when: hive_http_proxy is defined
 
 - name: create directory /etc/docker
   file:
     dest: "/etc/docker"
     state: directory
     mode: 0700
     owner: root
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dcp` & `hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/templates/dcp`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dexec` & `hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/templates/dexec`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client/templates/dsh` & `hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client/templates/dsh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/docker-client-proxy/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/drbd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/drbd/tasks/vg.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/drbd/tasks/vg.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/drbd-resource/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/drbd-resource/templates/volume.res` & `hive_builder-3.7.0/hive_builder/playbooks/roles/drbd-resource/templates/volume.res`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py` & `hive_builder-3.7.0/hive_builder/playbooks/roles/follow-swarm-service/files/follow-swarm-service.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/follow-swarm-service/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/tasks/build-gcp.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/tasks/create_instance.yml`

 * *Files 16% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         UserKnownHostsFile {{ hive_context_dir }}/known_hosts
         StrictHostKeyChecking yes
         User {{ hive_safe_admin }}
         PasswordAuthentication no
         IdentityFile {{ hive_safe_private_key_path }}
         IdentitiesOnly yes
         LogLevel FATAL
+      {% if hive_http_proxy is defined %}  RemoteForward {{ hive_http_proxy_port }} {{ hive_http_proxy }}{% endif %}
 - set_fact:
     hive_safe_disks:
     - auto_delete: True
       boot: True
       initialize_params:
         disk_size_gb: "{{ hostvars[gcp_host].hive_disk_size | default(25) }}"
         disk_name: "boot-{{ hive_safe_name }}"
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/tasks/destroy-gcp.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/gcp/vars/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/gcp/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/internal-network/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/internal-network/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/iptables/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/iptables/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/kickstart/tasks/main.yml`

 * *Files 2% similar despite different names*

```diff
@@ -106,10 +106,11 @@
         UserKnownHostsFile {{ hive_context_dir }}/known_hosts
         StrictHostKeyChecking yes
         User {{ hostvars[setup_host].hive_safe_admin }}
         PasswordAuthentication no
         IdentityFile {{ hive_safe_private_key_path }}
         IdentitiesOnly yes
         LogLevel FATAL
+      {% if hive_http_proxy is defined %}  RemoteForward {{ hive_http_proxy_port }} {{ hive_http_proxy }}{% endif %}
   loop: "{{ groups['servers'] | intersect(groups[hive_stage] )}}"
   loop_control:
     loop_var: setup_host
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2` & `hive_builder-3.7.0/hive_builder/playbooks/roles/kickstart/templates/kickstart.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/monitor-service-log/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2` & `hive_builder-3.7.0/hive_builder/playbooks/roles/monitor-service-log/templates/monitor-service-log.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/nfs-aws-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/nfs-azure-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/nfs-gcp-volumes/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/ntp-client/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/ntp-client/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/pip-venv/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/pip-venv/tasks/main.yml`

 * *Files 17% similar despite different names*

```diff
@@ -26,31 +26,25 @@
       - python{{ hive_safe_python_revision | split('.') | join('') }}-setuptools
       - "{{ 'python-virtualenv' if ansible_distribution == 'Amazon' else 'virtualenv' }}"
 - name: upgrade pip
   become: False
   pip:
     name:
       - pip
+      - setuptools
+      - wheel
     virtualenv: "{{ hive_home_dir }}/docker"
-    virtualenv_python: "{{ hive_safe_python_command }}"
+    virtualenv_command: python3 -m venv
     # hive-builder does not require libselinux module,
     # but inherit system site-pacakges for addon which requires libselinux module
     virtualenv_site_packages: "{{ hive_safe_need_libselinux }}"
-    extra_args: "{{ '-i ' + hive_pip_index_url if hive_pip_index_url is defined else omit }}"
+    extra_args: --disable-pip-version-check
     state: latest
   args:
     chdir: "{{ hive_home_dir }}"
-- name: set PyPi index url
-  become: False
-  copy:
-    content: |
-      [global]
-      index-url = {{ hive_pip_index_url }}
-    dest: "{{ hive_home_dir }}/docker/pip.conf"
-  when: hive_pip_index_url is defined
 - name: install python-dxf
   become: False
   pip:
     name:
       - python-dxf
     virtualenv: "{{ hive_home_dir }}/docker"
   args:
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/prepared/tasks/setup.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/prepared/tasks/setup.yml`

 * *Files 14% similar despite different names*

```diff
@@ -12,11 +12,12 @@
         UserKnownHostsFile {{ hive_context_dir }}/known_hosts
         StrictHostKeyChecking yes
         User {{ hostvars[setup_host].hive_safe_admin }}
         PasswordAuthentication no
         IdentityFile {{ hive_safe_private_key_path }}
         IdentitiesOnly yes
         LogLevel FATAL
+      {% if hive_http_proxy is defined %}  RemoteForward {{ hive_http_proxy_port }} {{ hive_http_proxy }}{% endif %}
   loop: "{{ hive_safe_hosts }}"
   loop_control:
     loop_var: setup_host
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/registry/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/registry/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/registry/templates/registry.yml.j2` & `hive_builder-3.7.0/hive_builder/playbooks/roles/registry/templates/registry.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/rsyslogd/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/rsyslogd/templates/services.conf` & `hive_builder-3.7.0/hive_builder/playbooks/roles/rsyslogd/templates/services.conf`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/service-backup/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/service-backup/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2` & `hive_builder-3.7.0/hive_builder/playbooks/roles/service-backup/templates/service-backup.sh.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/strict-source-ip/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/swarm/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/swarm/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/tls-certificate/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/users/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/users/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/files/Vagrantfile` & `hive_builder-3.7.0/hive_builder/playbooks/roles/vagrant/files/Vagrantfile`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/files/growfs.sh` & `hive_builder-3.7.0/hive_builder/playbooks/roles/vagrant/files/growfs.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/vagrant/tasks/main.yml`

 * *Files 4% similar despite different names*

```diff
@@ -48,8 +48,15 @@
     - not 'absent' in (groups['servers'] | intersect(groups[hive_stage]) | map('extract', hive_vagrant_result.status ))
     - not 'not_created' in (groups['servers'] | intersect(groups[hive_stage]) | map('extract', hive_vagrant_result.status ))
 - name: put ssh-config
   copy:
     content: "{{ hive_safe_vagrant_ssh_config.stdout }}"
     dest: "{{ hive_context_dir }}/ssh_config"
   when:
-    - not (hive_safe_vagrant_ssh_config.skipped | default(false))
+    - not (hive_safe_vagrant_ssh_config.skipped | default(false))
+- name: put RemoteForward setting
+  replace:
+    regexp: "^  User vagrant$"
+    replace: "  User vagrant\n  RemoteForward {{ hive_http_proxy_port }} {{ hive_http_proxy }}"
+    path: "{{ hive_context_dir }}/ssh_config"
+  when:
+    - hive_http_proxy is defined
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2` & `hive_builder-3.7.0/hive_builder/playbooks/roles/vagrant/templates/vagrant_vars.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/files/Template_App_systemd_Services.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/files/hive-repository-server.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/files/hive-server-selinux.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/files/hive-server.xml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/files/hive-server.xml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/tasks/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix/templates/zabbix.yml.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/docker-service.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/docker-volume-discover.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/hive.te` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/hive.te`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/hive.te.amzn`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/files/zbx_service_discovery.sh`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/tasks/main.yml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # setting retries to avoid following error on azure
 # fatal: [hive0.pdns]: FAILED! => changed=false
 #  msg: 'Failure downloading https://repo.zabbix.com/zabbix/3.0/rhel/7/x86_64/zabbix-release-3.0-1.el7.noarch.rpm, Request failed: <urlopen error [Errno 101] Network is unreachable>'
 #  results: []
 - name: Install Zabbix Repo
   yum:
-    name: https://repo.zabbix.com/zabbix/5.1/rhel/8/x86_64/zabbix-release-5.1-1.el8.noarch.rpm
+    name: http://repo.zabbix.com/zabbix/5.1/rhel/8/x86_64/zabbix-release-5.1-1.el8.noarch.rpm
     disable_gpg_check: true
     state: present
   until: not download_zabbix_repo.failed
   retries: 10
   delay: 5
   register: download_zabbix_repo
 - import_tasks: iptables.yml
@@ -29,34 +29,29 @@
     mode: 0775
     owner: zabbix
     group: zabbix
 - name: create virtual env for zabbix
   become_user: zabbix
   pip:
     name:
+      - setuptools
       - pip
+      - wheel
     virtualenv: /var/lib/zabbix/docker
-    virtualenv_python: "{{ hive_safe_python_command }}"
+    # virtualenv_python: "{{ hive_safe_python_command }}"
+    virtualenv_command: python3 -m venv
     # hive-builder does not require libselinux module,
     # but inherit system site-pacakges for addon which requires libselinux module
     virtualenv_site_packages: "{{ hive_safe_need_libselinux }}"
-    extra_args: "{{ '-i ' + hive_pip_index_url if hive_pip_index_url is defined else omit }}"
+    extra_args: --disable-pip-version-check
     state: latest
   args:
     chdir: /var/lib/zabbix
   vars:
     ansible_python_interpreter: "{{ '/usr/bin/python' if ansible_distribution == 'Amazon' else '/usr/libexec/platform-python' }}"
-- name: set PyPi index url for zabbix
-  become_user: zabbix
-  copy:
-    content: |
-      [global]
-      index-url = {{ hive_pip_index_url }}
-    dest: /var/lib/zabbix/docker/pip.conf
-  when: hive_pip_index_url is defined
 - name: install python pacages for zabbix
   become_user: zabbix
   pip:
     name:
       - wheel
       - docker
       - uptime
```

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/templates/docker-service.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/templates/zabbix_agentd.conf.j2`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml` & `hive_builder-3.7.0/hive_builder/playbooks/roles/zabbix-agent/vars/main.yml`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/playbooks/setup-hosts.yml` & `hive_builder-3.7.0/hive_builder/playbooks/setup-hosts.yml`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     # avoid error "The task includes an option with an undefined variable.
     # The error was: 'ansible_distribution' is undefined" when use --tags option
     - name: Gathering Facts when use tags option
       setup:
       tags: [ 'always' ]
       when: ansible_facts == {}
   roles:
+    - role: tls-certificate
+      tags: ["tls-certificate"]
     - role: base
       tags: ["base"]
     - role: hostsfile
       tags: ["hostsfile"]
     - role: ntp-client
       tags: ["ntp-client"]
       when: hive_ntp_servers is defined and hive_ntp_servers != omit
@@ -30,16 +32,14 @@
       when: hive_internal_net_if is defined
     - role: users
       tags: ["users"]
       when: hive_users is defined
     - role: strict-source-ip
       tags: ["strict-source-ip"]
       when: hive_ssh_source_ips is defined
-    - role: tls-certificate
-      tags: ["tls-certificate"]
     - role: docker
       tags: ["docker"]
     - role: drbd
       tags: ["drbd"]
       when: hive_mirrored_disk_size is defined
     - role: docker-client
       tags: ["docker-client"]
```

### Comparing `hive_builder-3.6.8/hive_builder/plugins/hive_inventory.py` & `hive_builder-3.7.0/hive_builder/plugins/hive_inventory.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/plugins/hive_services.py` & `hive_builder-3.7.0/hive_builder/plugins/hive_services.py`

 * *Files identical despite different names*

### Comparing `hive_builder-3.6.8/hive_builder/variables_metainf.yml` & `hive_builder-3.7.0/hive_builder/variables_metainf.yml`

 * *Files 6% similar despite different names*

```diff
@@ -358,7 +358,28 @@
   type: int
   default: 3
   name_in_ansible: hive_registry_backup_cleanup_days_before
 interpreter_python:
   description: "how to deside use which python interpretor"
   default: auto_silent
   name_in_ansible_cfg: interpreter_python
+http_proxy:
+  description: use http proxy for download software from public repository
+  name_in_ansible: hive_http_proxy
+  persistent_scope: stage
+http_proxy_port:
+  description: port number of proxy in servers
+  name_in_ansible: hive_http_proxy_port
+  default: '3128'
+  persistent_scope: stage
+registry_mirror:
+  description: mirror site URL for dockerhub registry
+  name_in_ansible: hive_registry_mirror
+  persistent_scope: stage
+pip_index_url:
+  description: index URL for pip
+  name_in_ansible: hive_pip_index_url
+  persistent_scope: stage
+pip_trusted_host:
+  description: trusted host for pip
+  name_in_ansible: hive_pip_trusted_host
+  persistent_scope: stage
```

### Comparing `hive_builder-3.6.8/pyproject.toml` & `hive_builder-3.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hive-builder"
-version = "3.6.8"
+version = "3.7.0"
 description = "Building docker swarm environment"
 authors = ["Mitsuru Nakakawaj <mitsuru@procube.jp>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "hive_builder"}]
 
 [tool.poetry.dependencies]
```

### Comparing `hive_builder-3.6.8/PKG-INFO` & `hive_builder-3.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hive-builder
-Version: 3.6.8
+Version: 3.7.0
 Summary: Building docker swarm environment
 License: MIT
 Author: Mitsuru Nakakawaj
 Author-email: mitsuru@procube.jp
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

