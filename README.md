Alfresco module which fixes an issue with external authentication in the following situation:
  When external authentication is enabled and a user is disabled, they are still allowed to authenticate.

It does so by overriding the beans for an external auth. subsystem called "external1", so the name
of your external subsystem in `authentication.chain` must be called "external1" for this module to do its work.
