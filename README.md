# PowerAutomateExpressions
List Rows action in Power Automate returns value and type column for Lookup columns, if we need to get text value then we have to use Get Row action, but we can get the text value without using the Get Row action using the Odata formatted values, just we need to put **@OData.Community.Display.V1.FormattedValue** to the end of the column name, for example there is a look column named Teacher in Student table
**_ms_teacher_value**  return Teacher Guid
**_ms_teacher_value@OData.Community.Display.V1.FormattedValue** returs Teacher Name
