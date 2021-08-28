# GuidGen

[GuidGen](https://green-bush-00b4eb210.azurestaticapps.net/) is a web app used to generate GUIDs.

Using the platform, one can generate any number of GUIDs.  

## How does it work

The web app is developed using Blazor. Using Web Assembly technology, it runs native C# code in the browser.  
Every time the user clicks on `Generate GUID` button, it executes the C# code `GUID.NewGuid()`.  
This is then deployed using `Azure Static Web Apps` offering.  
Every time a change is made, a new `workflow` is executed in `Github Actions`.  
This deploys the changes to `Azure Static Web Apps`.