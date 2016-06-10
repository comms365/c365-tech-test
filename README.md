# Comms365 Technical Test

This application will form the basis of a basic portal. To start the test please fork this repository and carry out the points below. Access to the resources should only be available via API using JSON.

## Tasks
* Create a user resource with sensible fields including a password that is stored appropiately. Please do manually rather than making use has_secure_password or any gems e.g. Devise. Include fields for email, first_name and last_name that are required.

* Implement a "soft delete" concern for models, such that if included the row is flagged as deleted instead of deleted. Apply to the user model with a default scope so that deleted rows are not queried.

* Allow API endpoints for the user resource to CRUD a user. User's can only update their own user.

## Caveats & Rules
### Database

Please use PostgreSQL as the database and apply relevant indexes. Assume all tables will contain many rows so indexing is critical.

### Testing

Use [RSpec](https://relishapp.com/rspec) and follow an outside-in testing approach. Approach testing your work in the same way you would during your day-to-day development.

### Quality Indicators

Please make use of quality indicators such as [CodeClimate](http://codeclimate.com), [Travis CI](travis-ci.com) and [Coveralls](https://coveralls.io). Update the provided badges in your `README.md` when setting up.