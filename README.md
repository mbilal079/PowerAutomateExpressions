# PowervAutomate Expressions
**Get Lookup column text value in List Rows Action** <br>
List Rows action in Power Automate returns value and type column for Lookup columns, if we need to get text value then we have to use Get Row action, but we can get the text value without using the Get Row action using the Odata formatted values, just we need to put **@OData.Community.Display.V1.FormattedValue** to the end of the column name, for example there is a look column named Teacher in Student table. <br>
**_ms_teacher_value**  return Teacher's guid. <br>
**_ms_teacher_value@OData.Community.Display.V1.FormattedValue** returns Teacher's Name. <br>

**Get the first row from For Each Control** <br>
Sometimes we need to get the first row only from the List Rows action, you can do it by the following expression. <br>
if(greater(length(outputs('List_Academic_Course'),0)),first(outputs('List_Academic_Course')?['value'])?['_mb_courseid_value'],null)


