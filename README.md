# SetParameter

This repository contains an automation script that can be used to trigger a parameter set on an element from a low code app.

## Input

The script requires the following input:

### ElementId [id: 2]

| Version | Description | Format | Example |
|:---|:---|:---| :---|
|Initial version| This should be used in the case that the element ID is set directly as input. | "DMA Id/Element Id" | 100/10 |
|1.0.0.1| Feed as an entry parameter for the element ID.| ["DMA Id/Element Id"]| ["100/10"]|

### ParameterId [id: 3]
	
The id of the write parameter (this can either be a standalone parameter or a table cell).

### PrimaryKey [id: 4]

The primary key in case a table cell needs to be set.
This needs to be formatted as a string array (example: ["key"]) and should be empty in case of a standalone parameter (example: []).

### Value [id: 5]

The value that needs to be set.
This needs to be formatted as a string array (example: ["value"]).
	
## Usage

This script can be used by providing hardcoded values as input or by using feeds in a low code app as shown in this example:

![Set Parameter Low Code app](/Documentation/SetParameter.png)
