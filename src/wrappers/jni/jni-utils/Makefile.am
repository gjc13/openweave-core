#
#    Copyright (c) 2014-2017 Nest Labs, Inc.
#    All rights reserved.
#
#    Licensed under the Apache License, Version 2.0 (the "License");
#    you may not use this file except in compliance with the License.
#    You may obtain a copy of the License at
#
#        http://www.apache.org/licenses/LICENSE-2.0
#
#    Unless required by applicable law or agreed to in writing, software
#    distributed under the License is distributed on an "AS IS" BASIS,
#    WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
#    See the License for the specific language governing permissions and
#    limitations under the License.
#

#
#    Description:
#      This file is the GNU automake template for the Nest Weave
#      utility classes for embedding Weave in a JVM
#

include $(abs_top_nlbuild_autotools_dir)/automake/pre.am

if WEAVE_WITH_JAVA

lib_LIBRARIES			     = libJNIUtils.a

libJNIUtils_a_SOURCES	             = \
    JNIUtils.cpp                       \
    $(NULL)

libJNIUtils_a_CPPFLAGS               = \
    -I$(top_srcdir)/src/include        \
    $(JNI_CPPFLAGS)                    \
    $(NULL)

#
# Local headers to build against and distribute but not to install
# since they are not part of the Weave SDK public API.
#
noinst_HEADERS                       = \
    JNIUtils.h                         \
    $(NULL)

endif # WEAVE_WITH_JAVA

include $(abs_top_nlbuild_autotools_dir)/automake/post.am
