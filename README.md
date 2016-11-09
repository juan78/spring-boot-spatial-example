# A Spring Boot example editing spatial data in MySQL

This is a small example app that shows how one can use

 * Spring Boot and Spring Data
 * Latest Hibernate with spatial features. The example uses more recent version than provided by Spring boms, to overcome some issues.
 * MySQL, which supports basic spatial types. If you want to run this example, prepare a "spatialdemo" database and possibly change DB credentials in src/main/resources/application.properties
 * Vaadin and V-Leaflet add-on to build the UI layer. With V-Leaflet we use the Editable extension and its Vaadin Field implementations which make it dead simple to edit JTS data types directly form the JPA entities.
 * As baselayer for maps OpenStreetMap layer is used, but naturally any common background map can be used.

...to build a full-stack web app handling spatial data efficiently.

As the data is now in an optimised form in the DB, it is possible to create efficient queries to the backend and e.g. only show features relevant to the current viewport of the map visualising features or what ever you can with MySQLs spatial queries.

Enjoy!