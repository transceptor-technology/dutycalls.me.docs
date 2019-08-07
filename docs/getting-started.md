# Getting started

## Overview

To start making use of our great product there are a few things that need to be done before any notification can be received by DutyCalls. These things are thoroughly described in the following steps.

## Step 1 - Create a workspace

### What is a workspace?

A workspace is a place where everything is done. As a user you have to be a member of a workspace to make use of the functionalities of DutyCalls. A workspace often represents a company or department. There are two ways of joining a workspace. You can get invited to one and you can create one yourself.

How can I create a workspace? That is very simple. Just sign in to DutyCalls and select the **Create workspace** card.

![image - Create a workspace - Step 1](/images/create-workspace-1.png)

Now enter a unique name for your workspace, click on the **Create** button and voila. Your workspace has been created.

![image - Create a workspace - Step 2](/images/create-workspace-2.png)

## Step 2 - Add a source

After you have signed in to your workspace, you have to add a source.

### What is a source?

A source is literally the source from where you receive notifications. It is probably the system that you want to connect to DutyCalls. You do not actually have to connect your system to DutyCalls, as it uses a REST API. But you must indicate what you are going to send. Notifications can of course be sent in any format and DutyCalls not how he should interpret these notifications.

To add a source you have to go to the sources page, click here on the **Add source** button.

![image - Add a source - Step 1](/images/add-source-1.png)

Here you will be asked for a name and then for a sample of a notification. This sample is just an example of a notification (must be valid JSON) from the system that you want to connect to DutyCalls. After pasting it, you can map all or your keys / values to the corresponding properties of a notification within DutyCalls. Lastly, click on the **Add** button and the source will be added to your workspace.

![image - Add a source - Step 2](/images/add-source-2.png)

As a result, DutyCalls knows how to display your notification. It is of course possible to disable some properties of a notification. It may of course be possible that, for example, you do not have to show a link in a notification or that for example no severity is included in a notification. There are, however, a number of mandatory fields. These are: `'channel'`, `'title'`, `'body'`, `'date / time'`.

## Step 3 - Add a channel

The next logical step is to add a channel.

### What is a channel?

A channel can be seen as a path a notification follows after being sent. Remember when adding the source, it was also mandatory to provide the name of a channel? All of the notifications from all of the sources that provide the same name will gather here. Users will be able to subscribe to these channels, what ensures that they also receive these notifications.

To add a channel. Go to the channels page and click on the **Add channel** button.

![image - Add a channel - Step 1](/images/add-channel-1.png)

You will have to fill in the following information:

* Name: The name of the new channel.
* Manager: A manager is ultimately responsible person within a channel and will, among other things, receive warnings when something is wrong within a channel. Every user within the workspace can be designated as a manager.
* Source: By selecting the source, the channel knows from source it must receive notifications.
* Schedules: Schedules or rather 'ignore schedules' are used to indicate when you do not want the channel to receive notifications. This does not have to be done immediately and can always be added / adjusted at a later stage. (optional)
* Status: The status indicates whether the channel is active or not. Only when a channel is active, it can receive notifications.

Now click on the **Add** button and the new channel will be added to your workspace.

![image - Add a channel - Step 2](/images/add-channel-2.png)

## Where to next?

Now that you have set up your workspace, you might want to check out these resources.

* Our [REST API Reference documentation](rest-api.md)
