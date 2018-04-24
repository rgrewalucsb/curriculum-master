# Singular `resource`s

In Rails' `routes.rb` file, we use the resources method to quickly declare all of the RESTful routes for a given controller.

Rails also provides us with a `resource` method we can use declare routes for resources we will access without `:id`s, that is, resources of which the user will only ever access one, and only one. In our auth pattern, we use a singular `resource` `session` because a user only interacts with one session (their own).

> NB: Although our routes may be "singular" when we declare them with `resource` we still follow the 'plural control names' convention; in this case, our controller is named `SessionsController` despite routing through `/session`. Controller names are always plural.

For more on this see the [Rails docs](http://guides.rubyonrails.org/routing.html#singular-resources).