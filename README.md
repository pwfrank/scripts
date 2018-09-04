# scripts

A collection of scripts used mostly for automating the backing up of personal files to an alternate storage volume and a remote storage service via cron.

##backup-anki
rsyncs anki folder on local volume to folder on alternate storage volume

##backup-aws

Recursively syncs selected directories on storage volume with dedicated AWS S3 bucket using AWS CLI tools (pip: awscli)

Dependencies: python, pip: awscli

n.b. you must append your python pip bin folder (~/.local/bin on arch) to your cron-specific path variable in order to execute via cron (i.e. prepend your crontab with the amended variable assignment)

##backup-linux
rsyncs various folders on local volume with storage volume

##charging-threshold-config
Wrapper for setting and reporting battery charge thresholds and charge/discharge states for the purpose of prolonging battery life. 

Dependencies: tpacpi-bat (acpi_call), tlp-stat. 

n.b. only suitable for Ivy Bridge and later-equipped ThinkPad models (xx30+), as earlier models utilize the tp_smapi utility )
