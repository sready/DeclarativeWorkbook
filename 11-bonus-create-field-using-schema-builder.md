# Module 11: Bonus - Create a Field using Schema Builder

Schema Builder provides a dynamic environment to add new custom objects, custom fields, and relationships to your schema. This eliminates the need to click from page to page to find the details of a master-detail relationship or to add a new custom field to an object in your schema. 

For example, if you’re using Schema Builder to view the details of your schema, you can add a new custom object without leaving Schema Builder. The drag-and-drop interface lets you easily add a custom object or new field, and saves the layout of your schema any time you move an object.

Schema Builder provides details such as the field values, required fields, and how objects are related by displaying lookup and master-detail relationships. You can view the details for both standard and custom objects in Schema Builder.


## Create a Field in the Schema Builder

1. Click **Setup** > **Customize** > **Schema Builder**

1. From the Objects Palette select the **Salesforce Request** and **User** objects.

![](https://raw.githubusercontent.com/sready/DeclarativeWorkbook/master/images/03-schema-builder-data-model.png)

1. Now let’s add an Admin Comments field using the Schema Builder. Click on the **Elements Tab**.

1. Then click and drag the `Long Text Field` from the Palette to the Salesforce Request Object.

![](https://raw.githubusercontent.com/sready/DeclarativeWorkbook/master/images/11-schema-builder-drag-field.png)

1. Fill in the details:
    Field Label: Admin Comments
    Length: 10,000

1. Click Save.


You have just added an Admin Comments field to the Salesforce request. Now let’s make sure that only Admins can see it.

1. Right click on the Admin Comments field and select Manage Field Permissions

1. Uncheck every box in the visible column by clicking Visible at the top twice.

![](https://raw.githubusercontent.com/sready/DeclarativeWorkbook/master/images/11-schema-builder-field-permissions.png)

1. Check only the System Administrator in the Visible column.

![](https://raw.githubusercontent.com/sready/DeclarativeWorkbook/master/images/11-schema-builder-field-permissions-admin-only.png)

1. Click Save.

Our field is now only visible to the Salesforce Admin. Fields you create via Schema Builder are not added to a page layout, so  you will need to add the field to the page layouts following the steps we used in the previous activities.
