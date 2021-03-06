package(default_visibility = ["//visibility:public"])

load(
    "@io_bazel_rules_go//go:def.bzl",
    "go_library",
)

go_library(
    name = "go_default_library",
    srcs = [
        "apparmor.go",
        "autoscaling_utils.go",
        "configmap.go",
        "configmap_volume.go",
        "container.go",
        "container_probe.go",
        "docker_containers.go",
        "downward_api.go",
        "downwardapi_volume.go",
        "empty_dir.go",
        "events.go",
        "expansion.go",
        "host_path.go",
        "init_container.go",
        "kubelet.go",
        "kubelet_etc_hosts.go",
        "lifecycle_hook.go",
        "networking.go",
        "node_lease.go",
        "pods.go",
        "privileged.go",
        "projected.go",
        "runtime.go",
        "secrets.go",
        "secrets_volume.go",
        "security_context.go",
        "sysctl.go",
        "ttlafterfinished.go",
        "util.go",
        "volumes.go",
    ],
    importpath = "k8s.io/kubernetes/test/e2e/common",
    deps = [
        "//pkg/api/v1/pod:go_default_library",
        "//pkg/apis/core:go_default_library",
        "//pkg/client/clientset_generated/internalclientset:go_default_library",
        "//pkg/client/conditions:go_default_library",
        "//pkg/kubelet:go_default_library",
        "//pkg/kubelet/apis:go_default_library",
        "//pkg/kubelet/images:go_default_library",
        "//pkg/kubelet/sysctl:go_default_library",
        "//pkg/security/apparmor:go_default_library",
        "//pkg/util/slice:go_default_library",
        "//pkg/util/version:go_default_library",
        "//staging/src/k8s.io/api/autoscaling/v1:go_default_library",
        "//staging/src/k8s.io/api/batch/v1:go_default_library",
        "//staging/src/k8s.io/api/coordination/v1beta1:go_default_library",
        "//staging/src/k8s.io/api/core/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/api/errors:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/api/resource:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/apis/meta/v1:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/fields:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/labels:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/runtime/schema:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/types:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/intstr:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/sets:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/uuid:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/util/wait:go_default_library",
        "//staging/src/k8s.io/apimachinery/pkg/watch:go_default_library",
        "//staging/src/k8s.io/client-go/kubernetes:go_default_library",
        "//staging/src/k8s.io/client-go/scale:go_default_library",
        "//staging/src/k8s.io/client-go/tools/cache:go_default_library",
        "//staging/src/k8s.io/client-go/tools/watch:go_default_library",
        "//test/e2e/framework:go_default_library",
        "//test/utils:go_default_library",
        "//test/utils/image:go_default_library",
        "//vendor/github.com/golang/glog:go_default_library",
        "//vendor/github.com/onsi/ginkgo:go_default_library",
        "//vendor/github.com/onsi/gomega:go_default_library",
        "//vendor/github.com/onsi/gomega/types:go_default_library",
        "//vendor/golang.org/x/net/websocket:go_default_library",
    ],
)

filegroup(
    name = "package-srcs",
    srcs = glob(["**"]),
    tags = ["automanaged"],
    visibility = ["//visibility:private"],
)

filegroup(
    name = "all-srcs",
    srcs = [":package-srcs"],
    tags = ["automanaged"],
)
