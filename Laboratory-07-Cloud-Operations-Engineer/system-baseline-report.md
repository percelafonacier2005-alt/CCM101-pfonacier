# System Baseline Report

## Introduction

This activity focuses on checking the initial health of a Linux server using the KillerCoda Ubuntu Playground. The purpose is to understand the available system resources before deploying a web application.

## Host System Baseline

### Memory Usage

Based on the free -h command, the server has *1.9 GiB of total RAM*, with 407 MiB currently used and 1.5 GiB available. This information helps determine whether the server has enough memory to handle additional workloads.

### Disk Storage

Based on the df -h / command, the root file system has a total capacity of *19 GB*. Around 5.5 GB is used, while 13 GB remains available. The current disk usage is 30%.

## Why Disk Space Monitoring Is Important

Checking disk space before a massive traffic surge helps ensure that the server has enough room to store application data and access logs, reducing the risk of service failures caused by insufficient storage.

