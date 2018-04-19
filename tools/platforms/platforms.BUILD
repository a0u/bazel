# Standard constraint_setting and constraint_values to be used in platforms.

package(
    default_visibility = ["//visibility:public"],
)

# These match values in //src/main/java/com/google/build/lib/util:CPU.java
constraint_setting(name = "cpu")

constraint_value(
    name = "x86_32",
    constraint_setting = ":cpu",
)

constraint_value(
    name = "x86_64",
    constraint_setting = ":cpu",
)

constraint_value(
    name = "ppc",
    constraint_setting = ":cpu",
)

constraint_value(
    name = "arm",
    constraint_setting = ":cpu",
)

constraint_value(
    name = "s390x",
    constraint_setting = ":cpu",
)

constraint_value(
    name = "riscv",
    constraint_setting = ":cpu",
)

# These match values in //src/main/java/com/google/build/lib/util:OS.java
constraint_setting(name = "os")

constraint_value(
    name = "osx",
    constraint_setting = ":os",
)

constraint_value(
    name = "freebsd",
    constraint_setting = ":os",
)

constraint_value(
    name = "linux",
    constraint_setting = ":os",
)

constraint_value(
    name = "windows",
    constraint_setting = ":os",
)

# A default platform with nothing defined.
platform(name = "default_platform")

# A default platform referring to the host system. This only exists for
# internal build configurations, and so shouldn't be accessed by other packages.
platform(
    name = "host_platform",
    cpu_constraints = [
        ":x86_32",
        ":x86_64",
        ":ppc",
        ":arm",
        ":s390x",
    ],
    host_platform = True,
    os_constraints = [
        ":osx",
        ":freebsd",
        ":linux",
        ":windows",
    ],
)

platform(
    name = "target_platform",
    cpu_constraints = [
        ":x86_32",
        ":x86_64",
        ":ppc",
        ":arm",
        ":s390x",
    ],
    os_constraints = [
        ":osx",
        ":freebsd",
        ":linux",
        ":windows",
    ],
    target_platform = True,
)
