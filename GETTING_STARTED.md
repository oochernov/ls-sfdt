# Instructions

These steps are required to take your cloned template to a functional gem.

1. Find and rename (case sensitive to preserve class names) **template** and **Template** file names and text from to the new gem name (i.e. for a new gem called 
logging, rename template to logging and Template to Logging).
1. Find and update all **TODO:** entries in the repo.
1. Install the dependencies `bundle install`.
1. Verify the tests pass locally `bundle exec rake`.
1. Check in any changes to local git (otherwise the gem/rake build will still reference them).
1. Verify the gem builds locally `bundle exec rake build`.
1. Push changes to the remote repository and ensure the main pipeline passes.
