# ue-css-cpp-httplib

The [cpp-httplib](https://github.com/yhirose/cpp-httplib) library for use with Satisfactory modding.

See [.artifact/usage.md](.artifact/usage.md) for usage information.

## Notes

Although cpp-httplib itself is header-only, it depends on either zlib or brotli for compression.
This build uses brotli since the choice is unlikely to make much difference in most cases,
brotli is the default of the vcpkg port, and the port does not currently expose `CPPHTTPLIB_ZLIB_SUPPORT`.

The brotli CLI tools are manually excluded from the package (see the Actions workflow in this repository)
since the vcpkg port does not currently provide a way to exclude them, and they should not bring in any extra dependencies.

## License

The licenses of cpp-httplib (MIT) and brotli (MIT) can be found alongside the binaries and headers
in the `share/**/copyright` files located within the release artifact.
