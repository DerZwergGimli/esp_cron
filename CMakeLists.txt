idf_component_register(
        SRCS "cron.c" "library/jobs/jobs.c" "library/ccronexpr/ccronexpr.c"
        INCLUDE_DIRS "include" "library/ccronexpr" "library/jobs")


target_compile_definitions(${COMPONENT_TARGET} PUBLIC -D CRON_USE_LOCAL_TIME)