# Index, Show, New, Create Lab

## Objectives

1. Build a RESTful index action
2. Build a RESTful show action
3. Build a RESTful new action
4. Build a RESTful create action
5. Interlink pages using route helpers
6. Use route helpers in redirect_to
7. Build a new form with form_tag


## Instructions

This will be a pretty extensive lab that will combine a number of the concepts that we have reviewed, including:

* Drawing multiple route types

* Integrating route helper methods

* Building out a form and wiring it up to the create action

* Linking pages together


In this lab the application you will be starting out with will be completely blank, there are no: models, views, controllers, etc. It has a number of RSpec and Capybara tests that will all need to pass to complete the lab. The tests can be found in the `specs` directory, in the `models`, `features`, and `controllers` directories. Feel free to walk through the specs to see what behavior the application should have when you're done.

The application you will be building will be a Coupon app. At a high level below are the features you will be building out:

* You will need to create a 'coupons' table with columns: `coupon_code` and `store`, which should both be of the `string` data type.

* Your index page should show all of the coupons in the database

* The coupon codes on the index page should link to their corresponding coupon show page, you should use the `link_to` and route helper methods instead of hard coding the HTML `<a>` tag

* Your `show` page should render the specific coupon passed to the route, e.g. `coupons/4` should show the coupon with an ID of 4

* The `new.html.erb` view template should render a form that uses the `form_tag` method

* The form should be wired up to the `create` action in the controller and when submitted should create a new record in the `coupons` table with the parameters passed through the form

* The form should use the `redirect_to` helper method to redirect the user to the `show` page template for that `coupon`


## Resources

* [Reading on Create Action](https://github.com/learn-co-curriculum/rails-create-action-readme)

* [Reading on Form Integration](https://github.com/learn-co-curriculum/rails-form_tag-readme)