# Microsoft Azure IoT Device SDK for C

## Introduction

The Microsoft Azure IoT device libraries for C contain code that facilitates building devices and applications that connect to and are managed by Azure IoT Hub services.

The device library consists of a set of reusable components with abstract interfaces that enable pluggability between stock and custom modules.

To meet the wide range of device requirements in the Internet of Things space, the C libraries are provided in source code form to support multiple form factors, operating systems, tools sets, protocols and communications patterns widely in use today.

## Features

* Sends event data to Azure IoT based services.

* Maps server commands to device functions.

* Buffers data when network connection is down.

* Batches messages to improve communication efficiency.

* Supports pluggable transport protocols. HTTP and AMQP protocols are available now, with more coming soon.

* Supports pluggable serialization methods. JSON is available now, with more coming soon.

## Tested platforms

The following platforms have been tested against this library:

* Windows 7

* Windows 8.1

* Ubuntu 14.04 LTS

* Debian 7.5

* Fedora 20

* Raspbian

* Mbed

The library code:

* Is written in ANSI C (C99) to maximize code portability.

* Avoids compiler extensions.

* Exposes a platform abstraction layer to isolate OS dependencies (HTTPAPI, Lock, Threads). Refer to the porting guide for more information.

