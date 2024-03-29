# Azure DevOps Work Connector
A [Visual Studio 2019 extension](https://marketplace.visualstudio.com/items?itemName=MadeUpExtensions.AzureDevopsWorkConnector)  allowing users to manage any Azure DevOps Work Items (Backlog Items, Bugs, Features etc.) from within Visual Studio.

By connecting to an Azure DevOps Project this extension allows a user within Visual Studio to Update an Assignee, Update the State, View & Add Comments and View the Description.

## Why Use it?
True Agile working requires great collaborative tools and up-to-date communication. Having the ability to update a Work Item from within Visual Studio means the whole team knows as soon as possible when a task is complete, blocked or ready for test, meaning time is saved regularly across all members of a project.

## How to use it
 1. First [install the extension](https://marketplace.visualstudio.com/items?itemName=MadeUpExtensions.AzureDevopsWorkConnector) from the Visual Studio market place.
 2. Once installed go to Tools > Options > Azure DevOps Work Connector
    and fill out the following settings:
    
	 1. **Azure DevOps instance URL**: The base URL of the Azure DevOps instance you want to connect to, this can be both the legacy and new URL structure.
	 2. **PAT Code**: Your Personal Access Token, found in [Azure DevOps](https://docs.microsoft.com/en-us/azure/devops/integrate/get-started/authentication/pats?view=azure-devops#create-personal-access-tokens-to-authenticate-access).
	 3. **Azure DevOps Assignee Name**: Your name as it appears in Azure DevOps, meaning that Work Items can be assigned to yourself in one click, and new comments appear under your name.
	 4. **Default Selected Work Item Types**: This is a comma seperated list of the Work Items Types that you want by default to be included in your WorkItem select list. This is defaulted to the following: 'Product Backlog Item,Bug'.
	 5. **Default Statuses Filter**: This is a comma seperated list of the Work Items Statuses that you want to IGNORE from your WorkItem select list. This is defaulted to the following: 'Done,Completed,Removed,Closed'.
	 6. **Default Selected WorkItem-Child Types Filter**: This is a comma seperated list of the WorkItems Child Types that you want to INCLUDE. This is defaulted to the following: 'Task,Bug'.
   
 3. To load the ADO Work Connector, in the toolbar, click View > Other Windows > Azure DevOps Work Connector, the connector will appear and can be docked in any pane, I recommend using it in a portrait pane.
 4. If steps 2.i and 2.ii have been completed correctly you will have a list of Projects available to select from the dropdown box. Select one
 5. Now you can either select a WorkItem, or filter your WorkItems further through either the Team/Iteration dropdown lists, WorkItem Type filters, WorkItem Statuses filters, WorkItem Title Filter and WorkItem Assignee Filter. The WorkItem Type & Statuses filters will both be set by default to any items you entered in part 2.iv and 2.v
 6. Once you have selected a Work Item all information and comments will be pulled down. You can now perform the following actions
	 1. **Assign yourself to the Work Item**: click the "Assign Myself" button.
	 2. **Assign someone to the Work Item**: click the "Assign To..." button and enter the assignee name as they appear in ADO.
	 3. **Select and Update a new State**: Use the State dropdown box to select the require state, and then click "Update State".
	 4. **Page through Comments**: Three comments are displayed at any one time, if more comments are available pagination options will appear below them, simply click "Previous" or "Next" to scroll through the comments.
	 5. **Add a new Comment**: To add a new comment first fill out the comments box, then click "Add Comment". The new comment will be displayed in the Comments section.
	 6. **Complete/Un-complete a sub workitem**: Sub workitems can be toggled to be complete or not by simply clicking on the tick box next to their name
	 7. **Add a new Task to the WorkItem**: Tasks can be added by clicking the Add new Task link, this will pop up an input box. Enter the title of your new task in the input box and click OK, this will refresh the WorkItem, allowing you to see the newly created task.
  
If you have any questions or suggestions please post them in the Q&A section.

**Coming Soon:**
1. Add a WorkItem
2. Increased error handling...
