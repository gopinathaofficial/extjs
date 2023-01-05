# Ext JS Preparation

**1.Layouts in ExtJs**
Ans : In Ext JS, layouts are used to define the arrangement of components within a container. Ext JS provides several built-in layout classes that you can use to create different types of layouts, including:

* HBox: A layout that arranges components horizontally in a single row.
* VBox: A layout that arranges components vertically in a single column.
* Fit: A layout that adjusts the size of a single component to fit the size of its container.
* Card: A layout that allows you to switch between multiple components, with only one component visible at a time.
* Accordion: A layout that arranges multiple components vertically, with the ability to expand and collapse each component.
* Border: A layout that divides a container into multiple regions, such as a north region, south region, east region, and west region.


You can use these layouts either as standalone layout objects, or you can set them as the layout for a container using the layout config.

For example:
```
Ext.create('Ext.panel.Panel', {
    title: 'My Panel',
    layout: 'vbox',
    items: [
        {xtype: 'component', html: 'Item 1'},
        {xtype: 'component', html: 'Item 2'},
        {xtype: 'component', html: 'Item 3'}
    ]
});
```
>This code creates a panel with a vertical box layout, which arranges the items in a single column.
