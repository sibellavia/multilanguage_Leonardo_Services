# Service Provisioning

Provisioning is one of the most important functionalities of SCMP. Through these modules, it is possible to allocate runtime assets within the providers managed by SCMP.

To use this functionality, relations must be defined within the SCMP.

This constraint was made available to bind certain characteristics to provisioning; for example, the VM size is not selectable during provisioning but is among the predefined characteristics by administrators within the catalog.

![Access to "Provisioning"](assets/images/extract/media/image6.png)

### Creation of Provisionings

#### Provisioning of "Physical Resources"

Using the tabs in the provisioning functionality, it is possible to view the lists of provisionable resources within the SCMP, such as Virtual Machines, Storage, and Kubernetes.

To view elements within the result lists, it is necessary that a relation exists in the SCMP catalog with the catalog resource of the provider to be provisioned.

The functionalities available for these elements are identical; only the parameters to be entered in the creation steps change.

![Tabs for resource creation](assets/images/extract/media/image290.png)

##### Virtual Machines

To start provisioning a resource, click on the corresponding row to view the page containing step 1 of provisioning creation. In this step, it is necessary to select, using the dropdown on the left, the "target" subsystem where the resources are to be provisioned. Once selected, an information mirror will be displayed on the right indicating the characteristics of the resource that will be provisioned. To continue, click the "Next" button at the bottom right to go to step 2 "Config" page.

![Selection of the “target” subsystem, provisioning step 1](assets/images/extract/media/image291.png)

On the "Config" page of step 2, fill in all mandatory fields in all sections of the form. At the bottom left, click the "Reset" button to reset all fields on the page.

Instead, on the right, click the "Submit" button to go to step 3 "Plan".

![](assets/images/extract/media/image292.png)
![Filling in the resource prediction form fields](assets/images/extract/media/image293.png)

After clicking the "Submit" button, the user is redirected to the "Plan" page of step 3 where we can view the provisioning plan sent by Terraform, which indicates all the parameters of the resources that will be configured, and at the bottom, there is a list with a cost perspective.

![Forecast screen](assets/images/extract/media/image294.png)

Still from the "Plan" page of step 3, at the bottom right, there are three buttons: "Back", "Reset", and "Apply". If you click the "Back" button, the user returns to the "Config" page of step 2 where parameters can be modified.

If you click the "Reset" button, the user is redirected to the "Subscription" page of step 1 where it is necessary to select a subsystem, and then enter the parameters on the "Config" page of step 2.

Finally, if you click the "Apply" button, the forecast is saved, and the user is redirected to the "Dashboard" tab page where the user verifies the presence of the newly created forecast.

![List of provisionings performed](assets/images/extract/media/image295.png)

#### Provisioning of "Services"

To access the services page, click on the tab that depicts a shelf located in the top menu. After doing this, you will find yourself on the "Service" page.

![List of cards](assets/images/extract/media/image296.png)

On the page, a list of components called "Card" is displayed. Each card refers to a specific type of service; in particular, the following information is displayed:

- Service name;
- Service icon;
- Type of script used for service provisioning;
- Service description;
- "Subscribe" button to proceed with service creation.

Depending on the type of service selected, the steps for provisioning change; these will be analyzed in detail below.

##### "Standard" Services

Click the "Subscribe" button corresponding to a "standard" service. The user will be redirected to step 1 of the service creation page, and all instantiable versions of the service by SCMP will be displayed. In particular, various blocks will be shown, each with a list of configurations:

- Name and version of the service that will be instantiated.
- Name and version of the operating system that will be installed on the machine.
- Belonging provider on which the service will be provisioned.

![Provisioning of a "standard" service](assets/images/extract/media/image297.png)

Select a software version and press the "Continue" button; the user is redirected to step 2 of service provisioning.

In step 2, it will be necessary to select a subsystem and fill out the form with the details of the chosen subsystem.

![Configuration of a "standard" service](assets/images/extract/media/image298.png)

After completing all the form fields, click "Submit".

A request will be sent to the Terraform service, which will validate the activation configuration of the indicated flow and return the result.

![Service configuration summary](assets/images/extract/media/image299.png)

Click "Apply" to validate the flow and activate the service subscription.

The dashboard page will open with the list of all subscribed services and their relative statuses. Specifically, the newly provisioned service will have a "Running" status in yellow, and subsequently, depending on the result, the status will also be updated to "Completed" in green or "Error" in red.

![Dashboard with the list of all subscribed services and their relative statuses](assets/images/extract/media/image300.png)

##### "Custom" Services

Click the "Subscribe" button corresponding to a "custom" service. The user will be redirected to step 1 of the service creation page where the subsystem can be selected, in which to perform the provisioning, from the dropdown in the center of the page.

![Provisioning of a “Custom” service](assets/images/extract/media/image301.png)

By selecting the subsystem, the page updates to proceed to step 2 of service provisioning.

In this step 2, it will be necessary to fill out the form with the specific configuration parameters of the selected service.

![Configuration of a "custom" service](assets/images/extract/media/image298.png)

After completing all the form fields, click "Launch".

A request will be sent to the Terraform service, which will validate the activation configuration of the indicated flow and return the result.

![Service configuration summary](assets/images/extract/media/image299.png)

Click "Apply" to validate the flow and start the automatic configuration operations.

The dashboard page will open with the list of all subscribed services and their relative statuses.

Specifically, the newly provisioned service will have a "Running" status in yellow, and subsequently, depending on the result, the status will also be updated to "Completed" in green or "Error" in red.

![Dashboard with the list of all subscribed services and their relative statuses](assets/images/extract/media/image300.png)

##### "Azure Pipeline" Services

Click the "Subscribe" button corresponding to an "Azure Pipeline" service. The user will be redirected to step 1 of the service creation page. From the dropdown in the center of the page, select the "Branch" of the pipeline to execute.

![Provisioning of an "Azure pipeline" service](assets/images/extract/media/image302.png)

By selecting the branch, the page updates to proceed to step 2 of service creation.

In this step 2, it will be necessary to fill out the form with the configuration parameters retrieved directly from the Pipeline that will be executed.

![Configuration of an "Azure pipeline" service](assets/images/extract/media/image303.png)

After completing all the form fields, click "Launch" to send the pipeline start request. The dashboard page will open with the list of all subscribed services and their relative statuses.

Specifically, the newly provisioned service will have a "Running" status in yellow, and subsequently, depending on the result, the status will also be updated to "Completed" in green or "Error" in red.

![Dashboard with the list of all subscribed services and their relative statuses](assets/images/extract/media/image300.png)

##### "PaaS" and "AI Services"

Click the "Subscribe" button corresponding to a "PaaS" service. The user will be redirected to step 1 of the service creation page where it will be necessary to fill out the form with the specific configuration parameters of the selected service.

![Configuration of a "PaaS" service](assets/images/extract/media/image304.png)

After completing all the form fields, click "Launch".

The dashboard page will open with the list of all subscribed services and their relative statuses.

Specifically, the newly provisioned service will have a "Running" status in yellow, and subsequently, depending on the result, the status will also be updated to "Completed" in green or "Error" in red.

![Dashboard with the list of all subscribed services and their relative statuses](assets/images/extract/media/image300.png)

##### "HELM" Services

Click the "Subscribe" button corresponding to a "HELM" service. The user will be redirected to step 1 of the service creation page where it will be necessary to select the cluster on which to perform the provisioning.

![Cluster selection](assets/images/extract/media/image305.png)

Fill out the form with the specific configuration parameters of the selected service. Also, add the "values.yaml" file at the bottom, which contains all the configuration parameters necessary for the service.

![Configuration of "HELM" parameters](assets/images/extract/media/image306.png)

After completing all the form fields, click "Launch".

The dashboard page will open with the list of all subscribed services and their relative statuses.

Specifically, the newly provisioned service will have a "Running" status in yellow, and subsequently, depending on the result, the status will also be updated to "Completed" in green or "Error" in red.

![Dashboard with the list of all subscribed services and their relative statuses](assets/images/extract/media/image300.png)

##### "Immutable" HELM Services

If the "immutable" flag was selected for the HELM service during creation, the user is not given the option to view and modify the service information, thus allowing for a "one-Click" installation.
Once "subscribe" is selected, the system automatically begins provisioning and returns the user to the dashboard page to monitor the results.

![Dashboard with the list of all subscribed services and their relative statuses](assets/images/extract/media/image300.png)

#### Modification of a performed provisioning

For a provisioning that has been carried out and has failed, it is possible to modify it.

Provisioning modification is only available for resource types.

To start modifying a provisioning, click on a failed forecast.

![Start modification of a Provisioning](assets/images/extract/media/image327.png)

After doing so, you will find yourself on the "Config" page of step 2 where you can modify the previously entered parameters.

![Configuration parameters](assets/images/extract/media/image328.png)

![Modification of parameters](assets/images/extract/media/image329.png)

After modifying the necessary parameters, at the bottom right, click the "Submit" button.

By doing so, you will find yourself on the "Plan" page of step 3, where the forecast is present, and below, the quote table.

At the bottom right, click the "Apply" button. After clicking the "Apply" button, you will find yourself on the "Dashboard" tab page.

Subsequently, from the "Dashboard" page, the user notes that the modification was successful.

It is also possible to modify a failed provisioning for other elements managed by SCMP.

![Provisioning summary and quote table](assets/images/extract/media/image330.png)
