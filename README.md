# ubc_saml_auth
A Drupal module which adds "protect by path" functionality to simplesamlphp_auth

/**
 * This module adds "protect by path" functionality to simplesamlphp_auth
 * 
 * For now, you need to hardcode your whitelisted paths
 * TODO: Create an admin UI for adding your whietlisted paths
 *
 * Note: This module currently works only on nodes. 
 * For Views, you can use Views access control to set the 
 * 'access cwl protected content'permission.
 *
 * Maintain your Whitelists in the following two functions:
 * ubc_saml_auth_getCWLWhitelist() for a list of whitelisted paths
 * ubc_saml_auth_pathIsInWildcardWhitelist() for a list of whitelisted wildcard rules
 */
