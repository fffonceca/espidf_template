file(GLOB_RECURSE srcs *.c)

set(include_dirs "."
                  "../include"
                  "../components/custom_foca/include"
                  "../components/custom_foca2/include")

idf_component_register(
    SRCS "${srcs}"
    INCLUDE_DIRS "${include_dirs}"
)
