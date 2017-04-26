# drupal_mpi_ldap_additions
A Drupal 7.x module to provide MPI specific code customisations to the Drupal LDAP module.

This module overrides the validation callback of the ldap_authentication module login 
form ('ldap_authentication_user_login_authenticate_validate'), in order to add the domain
"@mpi.nl" in case the user typed a username without domain. This allows MPI LDAP users to 
login by typing their internal MPI username only.
This module injects itself into Drupal's Authentication stack.
