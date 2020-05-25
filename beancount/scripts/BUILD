# TODO(blais): This file is incomplete.

package(default_visibility = ["//visibility:public"])

# py_library(
#     name = "bake",
#     srcs = ["bake.py"],
#     deps = [
#         "//beancount/utils:file_utils",
#         "//beancount/utils:version",
#         "//beancount/web:scrape",
#         "//beancount/web:web",
#     ],
# )

# py_test(
#     name = "bake_test",
#     srcs = ["bake_test.py"],
#     deps = [
#         "//beancount/scripts:bake",
#         "//beancount/utils:file_utils",
#         "//beancount/utils:test_utils",
#     ],
# )

py_test(
    name = "check_examples_test",
    srcs = ["check_examples_test.py"],
    deps = [
        "//beancount/scripts:check",
        "//beancount/utils:test_utils",
    ],
)

py_library(
    name = "check",
    srcs = ["check.py"],
    deps = [
        "//beancount:loader",
        "//beancount/ops:validation",
        "//beancount/utils:misc_utils",
        "//beancount/utils:version",
    ],
)

py_test(
    name = "check_test",
    srcs = ["check_test.py"],
    deps = [
        "//beancount/scripts:check",
        "//beancount/utils:test_utils",
        "//beancount:plugins_for_tests",
    ],
)

py_library(
    name = "deps",
    srcs = ["deps.py"],
    deps = [
    ],
)

py_test(
    name = "deps_test",
    srcs = ["deps_test.py"],
    deps = [
        "//beancount/scripts:deps",
    ],
)

py_library(
    name = "directories",
    srcs = ["directories.py"],
    deps = [
        "//beancount/core:account",
        "//beancount/core:getters",
    ],
)

py_test(
    name = "directories_test",
    srcs = ["directories_test.py"],
    deps = [
        "//beancount/scripts:directories",
    ],
)

# py_library(
#     name = "doctor",
#     srcs = ["doctor.py"],
#     deps = [
#         "//beancount/core:display_context",
#         "//beancount/utils:misc_utils",
#         "//beancount/utils:version",
#         "//beancount:loader",
#     ],
# )

# py_test(
#     name = "doctor_test",
#     srcs = ["doctor_test.py"],
#     deps = [
#         "//beancount/parser:cmptest",
#         "//beancount/scripts:directories_test",
#         "//beancount/scripts:doctor",
#         "//beancount/utils:test_utils",
#     ],
# )

py_library(
    name = "example",
    srcs = ["example.py"],
    deps = [
        "//beancount/core:account",
        "//beancount/core:amount",
        "//beancount/core:convert",
        "//beancount/core:data",
        "//beancount/core:display_context",
        "//beancount/core:getters",
        "//beancount/core:inventory",
        "//beancount/core:number",
        "//beancount/core:prices",
        "//beancount/core:realization",
        "//beancount:loader",
        "//beancount/ops:validation",
        "//beancount/parser:booking",
        "//beancount/parser:parser",
        "//beancount/parser:printer",
        "//beancount/scripts:format",
        "//beancount/utils:date_utils",
        "//beancount/utils:misc_utils",
        "//beancount/utils:version",
    ],
)

py_test(
    name = "example_test",
    srcs = ["example_test.py"],
    deps = [
        "//beancount:loader",
        "//beancount/ops:validation",
        "//beancount/scripts:example",
        "//beancount/utils:test_utils",
        "//beancount:plugins_for_tests",
    ],
)

py_library(
    name = "format",
    srcs = ["format.py"],
    deps = [
        "//beancount/core:account",
        "//beancount/core:amount",
        "//beancount/utils:version",
    ],
)

py_test(
    name = "format_test",
    srcs = ["format_test.py"],
    deps = [
        "//beancount/scripts:format",
        "//beancount/utils:test_utils",
    ],
)

# py_test(
#     name = "setup_test",
#     srcs = ["setup_test.py"],
#     deps = [
#         "//beancount/utils:test_utils",
#     ],
# )

py_library(
    name = "sql",
    srcs = ["sql.py"],
    deps = [
        "//beancount/core:data",
        "//beancount:loader",
        "//beancount/utils:misc_utils",
        "//beancount/utils:version",
    ],
)

py_test(
    name = "sql_test",
    srcs = ["sql_test.py"],
    deps = [
        "//beancount/scripts:sql",
        "//beancount/utils:test_utils",
    ],
)

py_library(
    name = "tutorial",
    srcs = ["tutorial.py"],
    deps = [
        "//beancount/utils:test_utils",
        "//beancount/utils:version",
    ],
)

# The problem with this test is that it calls the bean-report binary several times.
# You'll have to rework the test.
# py_test(
#     name = "tutorial_test",
#     srcs = ["tutorial_test.py"],
#     data = [
#         "//:example_beancount",
#     ],
#     deps = [
#         ":tutorial",
#         "//beancount/utils:test_utils",
#     ],
# )