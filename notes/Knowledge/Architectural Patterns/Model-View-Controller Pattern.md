# Model-View-Controller Pattern
[[User Interaction View]]

TODO: RAW: Pattern: Model-View-Controller
A system may offer multiple user interfaces. Each user interface depicts all or part of some
application data. Changes to the data should be automatically and flexibly reflected to all the
different user interfaces. It should be also possible to easily modify any one of the user interfaces, without affecting the application logic associated with the data.

The system is divided into three different parts: a Model that encapsulates some application data
and the logic that manipulates that data, independently of the user interfaces; one or multiple
Views that display a specific portion of the data to the user; a Controller associated with each
View that receives user input and translates it into a request to the Model. Views and Controllers
constitute the user interface. The users interact strictly through the Views and their Controllers,
independently of the Model, which in turn notifies all different user interfaces about updates.
