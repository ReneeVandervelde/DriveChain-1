DriveChain Changelog
====================

1.1.0
-----

This minor release focuses on improving the setup and ease of use for the 
framework.

 - Add `AppKernel` class to simplify imports and API for Application and Activity
   initialization calls.
 - Deprecate Application Lifecycle Subscriber Set kotlin extensions, to be 
   replaced with calls to `AppKernel`
 - Deprecate Lifecycle Registry Kotlin extensions, to be replaced with calls 
   to `AppKernel`
 - Add Lifecycle Voters to give libraries an automatic hook that can stop the 
   application initialization procedure. This is ueseful for bridges to 
   libraries with external application code such as LeakCanary 
 - Add a bridge for LeakCanary

1.0.1
-----
 - Fixed a Dependency loop error with the Logger Component.

1.0.0
-----
This release contained the initial buildout of the library framework including:

 - Application Lifecycle API
 - Activity Container Library
 - App Config API
 - Injectable Android Services for v26
 - Common Logger library
 - Library Bridges for Stetho, OkHttp and Fresco
