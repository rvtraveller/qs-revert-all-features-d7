# Revert All Features #

Revert all featuers in a Drupal 7 website using Quicksilver on Pantheon.

Note that with the current `webphp` type operations (currently the only option for Pantheon), your timeout is limited to 120 seconds, so long-running operations should be avoided for now. 


## Instructions ##

1. Require this Quicksilver module using composer (`composer require rvtraveller/qs-revert-all-features-d7`).
2. Add a Quicksilver operation to your `pantheon.yml` to fire the script before a deploy, using the example.pantheon.yml file for reference.  *Note:* you must set up your project's `composer.json` file to move projects of type `quicksilver-module` to the appropriate directory in your project.
3. Test a deploy out!

Optionally, you may want to use the `terminus workflows watch` command to get immediate debugging feedback.
