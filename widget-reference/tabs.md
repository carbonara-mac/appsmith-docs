---
description: >-
  The tabs widget is a special widget that contains multiple containers. Tabs
  can be used to contextually show UI to a user based on their choices.
---

# Tabs

![](../.gitbook/assets/tabs.gif)

## Creating Dynamic Views

You can create separate UIs in each tab container and dynamically switch between the containers by controlling the Default Tab property. The below code snippet demonstrates how you can control the selected tab based on the value the user sets in a dropdown 

```text
{{ Dropdown1.selectedOption === "1" ? "Tab1" : "Tab2" }}
```

## Properties

| Internal Property | Description |
| :--- | :--- |
| **selectedTab** | Contains the id of the tab currently selected |

| Widget Property | Description |
| :--- | :--- |
| **Tabs** | This property lets you add and remove tabs from the widget. Tabs are uniquely identified by their tab names  |
| **Default Tab** | This property selects the tab which matches the corresponding name |
| **Show Tabs** | This property hides / shows the tabs in the tab widget. It can be used to create the illusion of dynamically changing UI |
| **Scroll Contents** | This property enables scrolling within the contents of each tab  |
| **Visible** | Controls widget's visibility on the page. When turned off, the widget will not be visible when the app is published |

| Action | Description |
| :--- | :--- |
| **Column Action** | Adds a new column to the table with a button against each row. The button can be configured to trigger an action on the corresponding data row. |
| **onRowSelected** | Sets the action to be run when user selects a row in the table. Default supported actions are: Call API, Execute DB Query, Navigate to Page, Show Alert, Open / Close popup |
| **onPageChange** | Sets the action to be run when a table page is changed. Default supported actions are: Call API, Execute DB Query, Navigate to Page, Show Alert, Open / Close popup |
