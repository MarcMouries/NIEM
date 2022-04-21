# NIEM for ServiceNow

Extension of ServiceNow data model with selected elements from the National Information Exchange Model



| Domain        | Name          | Definition   | Notes
| ------------- | ------------- | ------------ | ------------- |
| Core          | Address       | A postal location to which paper mail can be directed.
| Core          | Case          | An aggregation of information about a set of related activities and events
| Core          | Entity        | A person, organization, or item
| Core          | Incident      | An occurrence or an event that may require a response. | Use the standard Incident table to manage unplanned          interruption to or quality reduction of an IT service. 
| Core          | Person        | A human being
| Core          | Organization  | A unit which conducts some sort of business or operation
| Core          | Request       | A formal message requesting something that is submitted to an authority.





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

| Property            | Definition   | Type               | NIEM Type.       | ServiceNow Type
| ----------------- | ------------- | ------------------- | ---------------- | -------------- 
| CaseYearDate      |  A year a case is opened.           |                  |
| CaseResolutionText|  A result of a case.                | (nc:TextType)
| CaseTitleText     |  An official name of a case.        | (nc:TextType)
| CaseTrackingID    |  An identifier used to track a case.| string




       
