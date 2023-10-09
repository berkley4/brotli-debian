# brotli-debian

This is a temporary measure until upstream debian update their package to v1.1.0 (see [1051575](https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=1051575)).

Not having this latest brotli release means that freetype (dependent on brotli), fontconfig (dependent on freeytype), and brotli itself cannot be unbundled.

I have been using these deb packages for building and running ungoogled chromium for the last couple of weeks without any noticable issues.

The build process runs a set of extensive self-tests which all complete without issue, further indicating that things function as intended.

The brotli and libbrotli-dev packages are needed to build ungoogled chromium with unbundled fontconfig and freetype.

The libbrotli1 package is needed to run the resulting build.
