# NIEM for ServiceNow


## OBJECTIVE:  
ServiceNow's objective is to be The Now Platform is the “Platform of Platforms”
To facilitate the automation of work across internal and external systems, it is crucial to extend ServiceNow core vocabulary so it's easier to communicate with those systems. 
NIEM, the National Information Exchange Model provides a common framework that is used to define how information can be shared between systems, government agencies and the private sector. It represents a collaborative partnership of agencies and organizations across all levels of government (federal, state, tribal, and local) and with private industry.

###Extension of ServiceNow data model with selected elements from the National Information Exchange Model


| Domain        | Name          | Definition   | Notes
| ------------- | ------------- | ------------ | ------------- |
| Core          | Address       | A postal location to which paper mail can be directed.
| Core          | Case          | An aggregation of information about a set of related activities and events
| Core          | Entity        | A person, organization, or item
| Core          | Incident      | An occurrence or an event that may require a response. | Use the standard Incident table to manage unplanned interruption to or quality reduction of an IT service. 
| Core          | Person        | A human being
| Core          | Organization  | A unit which conducts some sort of business or operation
| Core          | Request       | A formal message requesting something that is submitted to an authority.


## Person
A human being
| Property                  | Definition   | Type               | NIEM Type.       | ServiceNow Type
| ------------------------- | ------------- | ------------------- | ---------------- | -------------- 
| PersonBirthDate           | (nc:DateType)	| A date a person was born.
| PersonName                | (nc:PersonNameType) | A combination of names and/or titles by which a person is known. | We don't store the history of name changes
| PersonBirthDate           | (nc:DateType)	| A date a person was born.
| PersonFullName            |                    | A complete name of a person.
| PersonGivenName           |                    | A first name of a person.
| PersonJobTitleText        |                    | A title or label that briefly describes the position or kind of work a person does. | nc:TextType   | JobTitleText 
| PersonSurName             |                    | A last name or family name of a person.
| PersonNameSalutationText  |                    | A formal sign or expression of greeting that is appropriate for this person.
| PersonUSCitizenIndicator  |                    | True if a person is a citizen of the United States; false otherwise.




## Request
A data type for a formal message requesting something that is submitted to an authority.

| Property                  | Definition   | Type               | NIEM Type.       | ServiceNow Type
| ------------------------- | ------------- | ------------------- | ---------------- | -------------- 
| RequestContactInformation	| nc:ContactInformationType	    | A set of contact information for a point of contact for the request.
| RequestDate	              | nc:DateType	                  | A date on which a request was made.
| RequestDecisionText	| nc:TextType	                  | A decision that was made over a request.
| RequestDescriptionText	| nc:TextType		           | A description of a request.
| RequestIdentification	| nc:IdentificationType	    | An identification of a request.
| RequestText	              | nc:TextType		           | A request message.
| RequestDecisionDate	| nc:DateType		           | A date on which a decision was recorded for a request.
| RequestCategoryAbstract	| <abstract element, no type>   | A kind of request
| RequestStatus	       | nc:StatusType		    | A status of a request.
| RequestAugmentationPoint	| <abstract element, no type>.  | An augmentation point for RequestType.





## Case

| Property           | Definition                                     | Type             | NIEM Type.       | ServiceNow Column name
| ------------------ | ---------------------------------------------- | -----------------| ---------------- | -------------- 
| CaseYearDate       |  A year a case is opened.                      |                  |                  | u_caseyeardate
| CaseResolutionText |  A result of a case.                           | (nc:TextType)    |                  |
| CaseTitleText      |  An official name of a case.                   | (nc:TextType)    |                  |
| CaseTrackingID     |  An identifier used to track a case.           | string           |                  |
| CurrentMilestone   |  The current milestone                         |                  |                  |
| Milestones         |  Accomplishments during the execution of a case| List             |                  |




       
