java_binary(
    name = "ServerRunner",
    srcs = glob(["src/main/java/com/aleks/kv_store/*.java", "src/main/gen-java/com/aleks/kv_store/**/*.java"]),
    deps = [
        ":hello_gen",
        "@maven//:javax_annotation_javax_annotation_api",
        "@maven//:org_apache_thrift_libthrift",
        "@maven//:org_slf4j_slf4j_api",
        "@maven//:org_slf4j_slf4j_simple",
    ],
    main_class = "com.aleks.kv_store.KVServer",
)

genrule(
    name = "hello_gen",
    outs = ["hello2.txt"],
    srcs = ["src/main/thrift/com/aleks/kv_store/server.thrift"],
    cmd = "thrift --gen java -o src/main/ src/main/thrift/com/aleks/kv_store/server.thrift; echo hello world2 >$@",
)