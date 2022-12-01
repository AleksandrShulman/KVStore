java_binary(
    name = "ServerRunner",
    srcs = glob(["src/main/java/com/aleks/kv_store/*.java", "src/main/gen-java/com/aleks/kv_store/**/*.java"]),
    deps = [
        "@maven//:javax_annotation_javax_annotation_api",
        "@maven//:org_apache_thrift_libthrift",
        "@maven//:org_slf4j_slf4j_api",
        "@maven//:org_slf4j_slf4j_simple",
    ],
    main_class = "com.aleks.kv_store.KVServer",
)
