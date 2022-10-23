maincpp = ["dc.cpp"]

cc_library(
    name = "libdualcontour",
    srcs = glob(
        ["*.cpp"],
        exclude = maincpp + ["codeseg.cpp"],
    ),
    hdrs = glob(["*.h"]),
    # copts = ["-std=c++98"],
    includes = ["."],
    # linkopts = linkopts,
    # visibility = ["//:__pkg__"],
)

cc_binary(
    name = "dualcontour",
    srcs = maincpp,
    # copts = ["-std=c++98"],
    # linkopts = linkopts,
    deps = [":libdualcontour"],
)
