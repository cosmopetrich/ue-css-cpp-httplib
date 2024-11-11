# ue-css-cpp-httplib

The [cpp-httplib](https://github.com/yhirose/cpp-httplib) library for use with Satisfactory modding.

Although cpp-httplib itself is header-only, it depends on either zlib or brotli for compression.
This build uses brotli since the choice is unlikely to make much difference in most cases,
brotli is the default of the vcpkg port, and the port does not currently expose `CPPHTTPLIB_ZLIB_SUPPORT`.

See [.artifact/usage.md](.artifact/usage.md) for usage information.

## License

The licenses of cpp-httplib (MIT) and brotli (MIT) can be found alongside the binaries and headers
in the `share/**/copyright` files located within the release artifact.
