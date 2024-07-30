---
uid: Connector_help_Pro-Bel_Cygnus
---

# Pro-Bel Cygnus

This connector allows to monitor and configure the the Pro-Bel Cygnus routing system.

## About

This connector allows to monitor and configure the Pro-Bel Cygnus routing system, using smart-serial communication. The connector has two smart-serial connections which are set up as redundant polling.

### Version Info

| **Range** | **Description**      | **DCF Integration** | **Cassandra Compliant** |
|------------------|----------------------|---------------------|-------------------------|
| 1.0.0.x          | Initial version      | No                  | Yes                     |
| 2.0.0.x          | Smart Serial version | No                  | Yes                     |
| 3.0.0.x          | SNMP version         | No                  | Yes                     |


### Product Info

| Range | Supported Firmware Version |
|------------------|-----------------------------|
| 1.0.0.x          | -                           |
| 2.0.0.x          | -                           |
| 3.0.0.x          | -                           |

## Installation and configuration

### Creation

#### Serial connection - Main

SERIAL CONNECTION:

- Direct connection:

  - **Baudrate**: 38400
  - **Databits**: 8
  - **Stopbits**: 1
  - **Parity**: Even
  - **FlowControl**: *No*

- Interface connection:

  - **IP address/host**: The polling IP of the device.
  - **IP port**: The IP port of the device.
  - **Bus address**: 1

#### Serial connection - Secondary

SERIAL CONNECTION:

- Direct connection:

  - **Baudrate**: 38400
  - **Databits**: 8
  - **Stopbits**: 1
  - **Parity**: Even
  - **FlowControl**: *No*

- Interface connection:

  - **IP address/host**: The polling IP of the device.
  - **IP port**: The IP port of the device.
  - **Bus address**: 1

## Usage - Serial

### Matrix

This page gives an overview of the current matrix configuration. The number of inputs and outputs can be configured in the **Number of Inputs** and **Number of Outputs** parameters, respectively.

The Output Table gives an overview of which input is connected to which output.

### MON Overview

The **Set MON Name** parameter can be used to add an entry to the **MON Overview** table. Once an entry has been added to the **MON Overview** table, the **Output Table** will be polled.

### Advanced

This page allows to set advanced switching using the **Advanced Switching** parameter.

### Matrix Status

On this page an overview is given of the crosspoints (**Crosspoints**), the crosspoints buffer (**Crosspoints Buffer**), and status information (**Status Information** and **Communication Status**).

## Usage - SNMP

### General

This page gives an overview of the general information of the controller. The active status and the controller name.

### Matrices

This page gives an overview of the Matrices.

### Levels

This page gives an overview of the Levels this device has. The Index is made up of {Matrix Id}.{Level Id}

### Sources

This page gives an overview of the sources. The Index is made up of {Matrix Id}.{Level Id}.{Source Id}.
The display name of the sources can be configured using either the Alternative Name, 4 Character Name, 8 Character Name,  12 Character Name, or 16 Character Name. The format will be {Index}.{Choice}.\
The Enabled and Lock states are used in the Matrix.

#### Sources Association

This pages gives an overview of the sources association, and its relative association sources.

#### Sources Settings

This page allowes you to configure the sources table display key. Using either the Alternative Name, 4 Character Name, 8 Character Name,  12 Character Name, or 16 Character Name. The format will be {Index}.{Choice}.

### Destinations

This page gives an overview of the destinations. The Index is made up of {Matrix Id}.{Level Id}.{Destination Id}.
The display name of the destinations can be configured using either the Alternative Name, 4 Character Name, 8 Character Name,  12 Character Name, or 16 Character Name. The format will be {Index}.{Choice}.\
The Enabled and Lock states are used in the Matrix.

#### Destinations Settings

This page allowes you to configure the destinations table display key. Using either the Alternative Name, 4 Character Name, 8 Character Name,  12 Character Name, or 16 Character Name. The format will be {Index}.{Choice}.

### Matrix

This page shows the Matrix.
