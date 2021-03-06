# Traffic Monitor

## <font color = "blue">Objective</font> 
- Utilize AWS resources: <font color = "red">Lambda, S3, SQS, SNS.</font> 
- C# programming (.Net cross-platform)
- Xml and Json manipulation 
- Practicing Hybrid Model. 

## <font color = "blue">Description</font>

1. Collecting traffic image and filtering license plate. 
![Collection](/Asset/Collection.png)
2. Labelling metadata (Tag: **Key/Value**) for each license plate. 

|Tag|Description|
|------|--------|
|Location| Intersection address|
|Date/Time| Date and time the violation took place|
|Type| **no_stop, no_full_stop_on_right, no_right_on_red**|

*no_stop: $300*

*no_full_stop_on_right: $75*

*no_right_on_red*

3. Text Message Notification will have the following format 
Vehicle: **Color** **Make** **Model**
License plate: **PlateNumber**
Date: **The date/time the violation took place**
Violation address: **Address where the violation took place** Vilation type: **Type of violation**
Ticket amount: **The ticket amount**

## <font color = "blue">System Design </font>
![Design](/Asset/SystemWorkflowDiagram.png)

## <font color = "blue">Result </font>
![English](/Asset/English.png)
![Spanish](/Asset/Spanish.png)