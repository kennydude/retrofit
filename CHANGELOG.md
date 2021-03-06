Change Log
==========

Version 1.1.0 *(2013-06-20)*
----------------------------

 * Introduce `RequestInterceptor` to replace `RequestHeaders`. An interceptor provided to the
   `RestAdapter.Builder` will be called for every request and allow setting both headers and
   additional path parameter replacements.
 * Add `ErrorHandler` for customizing the exceptions which are thrown when synchronous methods
   return non-200 error codes.
 * Properly parse responses which erroneously omit the "Content-Type" header.


Version 1.0.2 *(2013-05-23)*
----------------------------

 * Allow uppercase letters in path replacement identifiers.
 * Fix: Static query parameters in the URL are now correctly appended with a separating '?'.
 * Fix: Explicitly allow or forbid `null` as a value for method parameters.
   * `@Path` - Forbidden
   * `@Query` - Allowed
   * `@Field` - Allowed
   * `@Part` - Forbidden
   * `@Body` - Forbidden
   * `@Header` - Allowed


Version 1.0.1 *(2013-05-13)*
----------------------------

 * Fix: Correct bad regex behavior on Android.


Version 1.0.0 *(2013-05-13)*
----------------------------

Initial release.
