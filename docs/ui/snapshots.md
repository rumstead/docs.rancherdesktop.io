---
sidebar_label: Snapshots
title: Snapshots
---

<head>
  <link rel="canonical" href="https://docs.rancherdesktop.io/ui/snapshots"/>
</head>

import TabsConstants from '@site/core/TabsConstants';


<!--- insert snapshot image -->
<Tabs groupId="os" defaultValue={TabsConstants.defaultOs}>
<TabItem value="Windows">

Windows_Image_TBD

</TabItem>
<TabItem value="macOS">

![Containers_Example](../img/Snapshot_Example.png)

</TabItem>
<TabItem value="Linux">

Linux_Image_TBD

</TabItem>
</Tabs>

A snapshot can be used to store the current configuration of your virtual machine and all associated settings. Snapshots are stored in a `snapshots` directory which are created at the below paths respective to your operating system:

- macOS: `~/Library/Application Support/rancher-desktop/snapshots`
- Linux: `~/.local/share/rancher-desktop/snapshots`
- Windows: `%LOCALAPPDATA%\rancher-desktop\snapshots`

The `snapshots` directory may be moved by creating a symlink from your system's default path to your preferred location.

### Snapshot Management

The following actions can be taken on the tab:

- `Create Snapshot`:
  You can choose to create a snapshot through the user interface from the Snapshots tab by clicking the `Create Snapshot` button. This will launch a dialog and provides a note alerting that Rancher Desktop will be unavailable during the creation of a new Snapshot.
  - `Snapshot Name`:
  Text can be entered into this field to name your snapshot.
  - `Description`:
  Text can be entered into the Description field that describes your snapshot.

- `Restore`:
  The `Restore` button can be used to restore a snapshot and will replace your current snapshot installation including preference settings. Rancher Desktop will be unavailable while this process is running.

- `Delete`:
  The `Delete` button can be used to remove snapshots permanently.

### Command Line - `rdctl snapshot`

All commands available through the user interface are also available using the `rdctl snapshot` command. Please see the [reference page](https://docs.rancherdesktop.io/references/rdctl-command-reference) for more information.