@kazuhitoyokoi/node-red-contrib-patlite
=====================

A node to control Patlite NHV series

## Install

Run the following command in your Node-RED user directory - typically `~/.node-red`

        npm install @kazuhitoyokoi/node-red-contrib-patlite

After setting the IP address and target (light color or buzzer) in the node property, you can control this node with the `msg.payload` value.

### Input
- `msg.payload` _boolean_

  If the received `msg.payload` is `true`, the target light will be on.
  When `msg.payload` has `false` value, the target light is turned off.

- `msg.topic` _number_

  You can set the light or buzzer mode in the `msg.topic`.
  The range of the value is between `1` and `5`.

### Settings
To allow this node to access the HTTP server on your Patlite device, you need to enable the HTTP Command Control in advance.

![](https://github.com/kazuhitoyokoi/node-red-contrib-patlite/blob/main/settings.png)

### Demonstrations
- Simple flow demonstration

  ![](https://github.com/kazuhitoyokoi/node-red-contrib-patlite/blob/main/demo.gif)

- Dashboard integration

  ![](https://github.com/kazuhitoyokoi/node-red-contrib-patlite/blob/main/dashboard.gif)
