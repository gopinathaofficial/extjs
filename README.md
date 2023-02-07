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

**2.What is MVC and MVMM?**

Ans : Model-View-Controller (MVC) and Model-View-ViewModel (MVVM) are both architectural patterns for designing software applications. Both patterns are designed to separate the user interface (UI) from the business logic of the application, making it easier to develop and maintain the application over time.

MVC is a design pattern that separates an application into three main components: the model, the view, and the controller. The model represents the data and business logic of the application, the view represents the UI, and the controller serves as the intermediary between the model and the view.

MVVM is a variation of MVC that was specifically designed for use with rich client-side applications, such as those built with WPF (Windows Presentation Foundation) or Ext JS. In MVVM, the view model acts as the intermediary between the view and the model, providing data-binding and other features to facilitate communication between the two.

Both MVC and MVVM are popular patterns for building modern web applications, and both have their own strengths and weaknesses. In general, MVC is a good choice for applications with simple UI requirements, while MVVM is better suited to applications with more complex UI needs.

**3.What is MVC Architecture?**

Ans: Model-View-Controller (MVC) is an architectural pattern that separates an application into three main components: the model, the view, and the controller. These components are designed to work together to create a web application that is flexible, maintainable, and easy to develop.

The model represents the data and business logic of the application. It is responsible for managing the data and performing any necessary calculations or processing.

The view represents the user interface (UI) of the application. It is responsible for rendering the UI and presenting the data to the user.

The controller is the intermediary between the model and the view. It receives user input and requests, and then uses the model to process these requests and generate the appropriate response. The controller then sends the response back to the view, which updates the UI to reflect the changes.

MVC is a popular pattern for building modern web applications because it helps to separate the UI from the business logic of the application, making it easier to develop and maintain the application over time.

**4.How to communicate between crontrollers?**

Ans: In ExtJS, there are several ways to communicate between controllers. Some of the most common methods include:

Using a shared service: A shared service can be used to share data between controllers. This is a useful method when multiple controllers need to access the same data or when data needs to be passed between controllers.

Using events: ExtJS controllers can fire and listen to events. This allows one controller to notify another controller of an event that has occurred. For example, a 'save' button click in one controller can fire an event that is listened to by another controller to update a grid.

Using global events: ExtJS global events provide a way for different controllers to communicate with each other without the need for direct references. For example, one controller can fire a global event 'userloggedin' and another controller can listen to it.

Using a parent-child relationship: Some controllers can have a parent-child relationship, where a parent controller has access to the child controller's methods and properties. This allows for easy communication between the two controllers.

Using references: You can use references config in controller to get reference of other component and by using that component reference you can access other component methods and properties.

Using ViewModel: You can use viewmodel to share data between different controllers.

It depends on the specific use case, you can choose the most appropriate method for your application.

**5. How to generate Extjs application from SDK?**

Ans: 
Steps:
1) Download the SDK and extract the zip file.

2) sencha -sdk "SDK path" generate app modern or classic appname path where we need to generate the application 
(eg:sencha -sdk "D:\hitachi\ext-7.5.1\ext-7.5.1" generate app modern sevenpointzero D:/hitachi/sevenpointzero).

3) after generation run the app using **sencha app watch**



