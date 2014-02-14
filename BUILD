[
  { "cc_library": {
      "name": "vina_lib",
      "cc_sources": [ "src/lib/*.cpp" ],
      "cc_headers": [ "src/lib/*.h" ],
      "dependencies": [ "//third_party/boost:system",
                        "//third_party/boost:thread",
                        "//third_party/boost:serialization",
                        "//third_party/boost:filesystem",
                        "//third_party/boost:program_options" ],
      "cc_linker_args": [ "-lpthread" ],
      "header_compile_args": [ "-Wno-error=reorder" ],
      "licenses": [ "http://opensource.org/licenses/Apache-2.0" ]
  } },
  { "cc_binary": {
      "name": "vina",
      "cc_sources": [ "src/main/main.cpp" ],
      "cc_include_dirs": [ "src/lib" ],
      "dependencies": [ ":vina_lib" ]
  } }
]