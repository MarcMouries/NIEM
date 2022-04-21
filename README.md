# NIEM for ServiceNow

Extension of ServiceNow data model with selected elements from the National Information Exchange Model



| Domain        | Name          | Definition   | Notes
| ------------- | ------------- | ------------ | ------------- |
| Core          | Entity        | A person, organization, or item
| Core          | Person        | A human being
| Core          | Organization  | A unit which conducts some sort of business or operation
| Core          | Case          | An aggregation of information about a set of related activities and events
| Core          | Incident      | An occurrence or an event that may require a response. | Use the standard Incident table to manage unplanned          interruption to or quality reduction of an IT service. 
| Core          | Address       | A postal location to which paper mail can be directed.


## Case

| Property            | Definition   | Type               | NIEM Type.       | ServiceNow Type
| ----------------- | ------------- | ------------------- | ---------------- | -------------- 
| CaseYearDate      |  A year a case is opened.           |                  |
| CaseResolutionText|  A result of a case.                | (nc:TextType)
| CaseTitleText     |  An official name of a case.        | (nc:TextType)
| CaseTrackingID    |  An identifier used to track a case.| string




       
