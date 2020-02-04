# ubc_saml_auth
A Drupal module which adds "protect by path" functionality to simplesamlphp_auth

/**
 * This module adds "protect by path" functionality to simplesamlphp_auth
 * 
 * Note: This module currently works only on nodes. 
 * For Views, you can use Views access control to set the 
 * 'access cwl protected content'permission.
 *
 * Maintain your Whitelists in the following two functions:
 * ubc_saml_auth_getCWLWhitelist() for a list of whitelisted paths
 * ubc_saml_auth_pathIsInWildcardWhitelist() for a list of whitelisted wildcard rules
 */

# Cron Error
You may encounter an issue running cron from the Status Report page.  Cron and drupal_goto calls don't always play nicely together, but the drupal_goto call on line 134 is handled correctly according to Drupal.org issue queues.  You can run cron from the Status Report page using the "run cron manually" link, however the link with the cron_key may not work.  Most importantly however is that cron will run correctly from the server.
