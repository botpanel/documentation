# Bot Panel Documentation

This documentation assumes that you have already installed [BotPanel](https://dev.botpanel.xyz). If you have not already, you can find the instructions for doing so below

[Bot Panel w/ Bot Maker for Discord Integration Guide](https://github.com/botpanel/bmd)<br>
[Bot Panel w/ Discord Bot Maker Integration Guide](https://github.com/botpanel/dbm)

* [More on Vanity URLs](https://github.com/botpanel/documentation/edit/main/README.md#more-on-vanity-urls)
* [Input Components](https://github.com/botpanel/documentation/edit/main/README.md#input-components)
   * [Text Input Components](https://github.com/botpanel/documentation/edit/main/README.md#text-input-components)

# More on Vanity URLs

Vanity URLs are what your users use to access your bot, however your user dashboard is also accessible by using its application id in place of the vanity url. For example:

`https://botpanel.xyz/dashboard/VANITY_URL` -> `https://botpanel.xyz/dashboard/APPLICATION_ID`

As application IDs are unique UUIDv4 strings, vanity URLs are not allowed to match said pattern. Additionally all vanity URLs must only consist of alphanumerics, underscores, or dashes.

# Input Components

Input components are what allow you to give your users the permission of changing specific values in your bot. There are several types of Input Components, each with their own unique set of parameters.

When clicking the `Add component` button on your user dashboard editor, a modal will pop up with these required options that are shared among all input components:

| Field Name    | Description                                                                                                                                                                                                                                                                                                                                             |
|---------------|---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Name          | This is the name of the input component, and will be displayed in a large header.                                                                                                                                                                                                                                                                       |
| Description   | This is the description of the input component, displayed under the header in smaller font.                                                                                                                                                                                                                                                             |
| Variable Name | This is the name of the server variable that the input component will be stored into. For example: if I have a string input component with the variable name `welcomeMessage`, then when the value is saved from the user dashboard, the server data for the selected guild with name `welcomeMessage` will be updated to the value from the dashboard. |
| Input Type    | Input type for the component.                                                                                                                                                                                                                                                                                                                           |

## Text Input Components

The Text Input Component is used for collecting strings of data, or text.
