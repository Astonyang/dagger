# Copyright (C) 2018 The Dagger Authors.
#
# Licensed under the Apache License, Version 2.0 (the "License");
# you may not use this file except in compliance with the License.
# You may obtain a copy of the License at
#
# http://www.apache.org/licenses/LICENSE-2.0
#
# Unless required by applicable law or agreed to in writing, software
# distributed under the License is distributed on an "AS IS" BASIS,
# WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
# See the License for the specific language governing permissions and
# limitations under the License.

# Description:
#   The Service Provider Interface for Dagger's binding graph model

package(default_visibility = ["//:src"])

load(
    "//:build_defs.bzl",
    "DOCLINT_HTML_AND_SYNTAX",
    "DOCLINT_REFERENCES",
)

filegroup(
    name = "spi-srcs",
    srcs = glob(["*.java"]),
)

java_library(
    name = "spi",
    srcs = [":spi-srcs"],
    javacopts = DOCLINT_HTML_AND_SYNTAX + DOCLINT_REFERENCES,
    deps = [
        "//java/dagger:core",
        "//java/dagger/model",
        "//third_party:auto_value",
        "//third_party:error_prone_annotations",
        "//third_party:guava",
        "//third_party:jsr330_inject",
    ],
)
