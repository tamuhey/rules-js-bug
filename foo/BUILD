load("@npm//:defs.bzl", "npm_link_all_packages")
load("@npm//foo:typescript/package_json.bzl", typescript = "bin")

npm_link_all_packages()

typescript.tsc(
    name = "foo",
    outs = ["src/Foo.js"],
    chdir = package_name(),
    srcs = [
        "src/Foo.tsx",
        "tsconfig.json",
        "//foo:node_modules/@headlessui/react",
        "//foo:node_modules/@types/react",
        "//foo:node_modules/@types/react-dom",
        "//foo:node_modules/react",
        "//foo:node_modules/react-dom",
    ],
)
