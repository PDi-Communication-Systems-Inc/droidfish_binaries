This is a temporary repository until we can build Droidfish from source. The main barrier is finding a way to include a full-feature C++ STL codebase from within the AOSP build system. The stlport exernal project does not include all the necessary STL classes needed for a full build. Also, some specialized data files cannot easily be placed into the root of the apk archive (They can be placed into assets and the source modified). 

In Marshmallow, it is possible to specify a NDK C++ STL library to use that should work around this.
