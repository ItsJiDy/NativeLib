# For more information about using CMake with Android Studio, read the
# documentation: https://d.android.com/studio/projects/add-native-code.html

# Sets the minimum version of CMake required to build the native library.

cmake_minimum_required(VERSION 3.18.1)

# Declares and names the project.

project("MyLibName" CXX)

# Creates and names a library, sets it as either STATIC
# or SHARED, and provides the relative paths to its source code.
# You can define multiple libraries, and CMake builds them for you.
# Gradle automatically packages shared libraries with your APK.

add_library( # Sets the name of the library.
        mobileblox

        # Sets the library as a shared library.
        SHARED

        # Provides a relative path to your source file(s).
        NativeLib/utils/utils.cpp
        NativeLib/roblox/hooks.cpp
        NativeLib/main.cpp
        NativeLib/exploit.cpp
        NativeLib/dependencies/luau/Ast/src/Ast.cpp
        NativeLib/dependencies/luau/Ast/src/Confusables.cpp
        NativeLib/dependencies/luau/Ast/src/Lexer.cpp
        NativeLib/dependencies/luau/Ast/src/Location.cpp
        NativeLib/dependencies/luau/Ast/src/Parser.cpp
        NativeLib/dependencies/luau/Ast/src/StringUtils.cpp
        NativeLib/dependencies/luau/Ast/src/TimeTrace.cpp
        NativeLib/dependencies/luau/Compiler/src/BuiltinFolding.cpp
        NativeLib/dependencies/luau/Compiler/src/Builtins.cpp
        NativeLib/dependencies/luau/Compiler/src/BytecodeBuilder.cpp
        NativeLib/dependencies/luau/Compiler/src/Compiler.cpp
        NativeLib/dependencies/luau/Compiler/src/ConstantFolding.cpp
        NativeLib/dependencies/luau/Compiler/src/CostModel.cpp
        NativeLib/dependencies/luau/Compiler/src/lcode.cpp
        NativeLib/dependencies/luau/Compiler/src/TableShape.cpp
        NativeLib/dependencies/luau/Compiler/src/Types.cpp
        NativeLib/dependencies/luau/Compiler/src/ValueTracking.cpp
        NativeLib/dependencies/luau/VM/src/lapi.cpp
        NativeLib/dependencies/luau/VM/src/laux.cpp
        NativeLib/dependencies/luau/VM/src/lbaselib.cpp
        NativeLib/dependencies/luau/VM/src/lbitlib.cpp
        NativeLib/dependencies/luau/VM/src/lbuiltins.cpp
        NativeLib/dependencies/luau/VM/src/lcorolib.cpp
        NativeLib/dependencies/luau/VM/src/ldblib.cpp
        NativeLib/dependencies/luau/VM/src/ldebug.cpp
        NativeLib/dependencies/luau/VM/src/ldo.cpp
        NativeLib/dependencies/luau/VM/src/lfunc.cpp
        NativeLib/dependencies/luau/VM/src/lgc.cpp
        NativeLib/dependencies/luau/VM/src/lgcdebug.cpp
        NativeLib/dependencies/luau/VM/src/linit.cpp
        NativeLib/dependencies/luau/VM/src/lmathlib.cpp
        NativeLib/dependencies/luau/VM/src/lmem.cpp
        NativeLib/dependencies/luau/VM/src/lnumprint.cpp
        NativeLib/dependencies/luau/VM/src/lobject.cpp
        NativeLib/dependencies/luau/VM/src/loslib.cpp
        NativeLib/dependencies/luau/VM/src/lperf.cpp
        NativeLib/dependencies/luau/VM/src/lstate.cpp
        NativeLib/dependencies/luau/VM/src/lstring.cpp
        NativeLib/dependencies/luau/VM/src/lstrlib.cpp
        NativeLib/dependencies/luau/VM/src/ltable.cpp
        NativeLib/dependencies/luau/VM/src/ltablib.cpp
        NativeLib/dependencies/luau/VM/src/ltm.cpp
        NativeLib/dependencies/luau/VM/src/ludata.cpp
        NativeLib/dependencies/luau/VM/src/lutf8lib.cpp
        NativeLib/dependencies/luau/VM/src/lvmexecute.cpp
        NativeLib/dependencies/luau/VM/src/lvmload.cpp
        NativeLib/dependencies/luau/VM/src/lvmutils.cpp
        NativeLib/roblox/update.cpp
        NativeLib/execution/execution.cpp
        NativeLib/environment/libraries/misc.cpp
        NativeLib/environment/environment.cpp
        NativeLib/taskscheduler/taskscheduler.cpp
        NativeLib/callcheck/callcheck.cpp
        NativeLib/dependencies/cpr/auth.cpp
        NativeLib/dependencies/cpr/cookies.cpp
        NativeLib/dependencies/cpr/cprtypes.cpp
        NativeLib/dependencies/cpr/digest.cpp
        NativeLib/dependencies/cpr/error.cpp
        NativeLib/dependencies/cpr/multipart.cpp
        NativeLib/dependencies/cpr/parameters.cpp
        NativeLib/dependencies/cpr/payload.cpp
        NativeLib/dependencies/cpr/proxies.cpp
        NativeLib/dependencies/cpr/session.cpp
        NativeLib/dependencies/cpr/ssl_options.cpp
        NativeLib/dependencies/cpr/timeout.cpp
        NativeLib/dependencies/cpr/util.cpp
        NativeLib/dependencies/imgui/backends/imgui_impl_android.cpp
        NativeLib/dependencies/imgui/backends/imgui_impl_opengl3.cpp
        NativeLib/dependencies/imgui/imgui.cpp
        NativeLib/dependencies/imgui/imgui_demo.cpp
        NativeLib/dependencies/imgui/imgui_draw.cpp
        NativeLib/dependencies/imgui/imgui_tables.cpp
        NativeLib/dependencies/imgui/imgui_widgets.cpp
        NativeLib/dependencies/luau/VM/src/lbuffer.cpp
        NativeLib/dependencies/luau/VM/src/lbuflib.cpp
        NativeLib/dependencies/lz4/lz4.cpp
        NativeLib/environment/libraries/closure.cpp
        NativeLib/reflection/instance.cpp
        NativeLib/renderer/renderer.cpp
        NativeLib/dependencies/ixwebsocket/IXBench.cpp
        NativeLib/dependencies/ixwebsocket/IXCancellationRequest.cpp
        NativeLib/dependencies/ixwebsocket/IXConnectionState.cpp
        NativeLib/dependencies/ixwebsocket/IXDNSLookup.cpp
        NativeLib/dependencies/ixwebsocket/IXExponentialBackoff.cpp
        NativeLib/dependencies/ixwebsocket/IXGetFreePort.cpp
        NativeLib/dependencies/ixwebsocket/IXGzipCodec.cpp
        NativeLib/dependencies/ixwebsocket/IXHttp.cpp
        NativeLib/dependencies/ixwebsocket/IXHttpClient.cpp
        NativeLib/dependencies/ixwebsocket/IXHttpServer.cpp
        NativeLib/dependencies/ixwebsocket/IXNetSystem.cpp
        NativeLib/dependencies/ixwebsocket/IXSelectInterrupt.cpp
        NativeLib/dependencies/ixwebsocket/IXSelectInterruptEvent.cpp
        NativeLib/dependencies/ixwebsocket/IXSelectInterruptFactory.cpp
        NativeLib/dependencies/ixwebsocket/IXSelectInterruptPipe.cpp
        NativeLib/dependencies/ixwebsocket/IXSetThreadName.cpp
        NativeLib/dependencies/ixwebsocket/IXSocket.cpp
        NativeLib/dependencies/ixwebsocket/IXSocketAppleSSL.cpp
        NativeLib/dependencies/ixwebsocket/IXSocketConnect.cpp
        NativeLib/dependencies/ixwebsocket/IXSocketFactory.cpp
        NativeLib/dependencies/ixwebsocket/IXSocketMbedTLS.cpp
        NativeLib/dependencies/ixwebsocket/IXSocketOpenSSL.cpp
        NativeLib/dependencies/ixwebsocket/IXSocketServer.cpp
        NativeLib/dependencies/ixwebsocket/IXSocketTLSOptions.cpp
        NativeLib/dependencies/ixwebsocket/IXStrCaseCompare.cpp
        NativeLib/dependencies/ixwebsocket/IXUdpSocket.cpp
        NativeLib/dependencies/ixwebsocket/IXUrlParser.cpp
        NativeLib/dependencies/ixwebsocket/IXUserAgent.cpp
        NativeLib/dependencies/ixwebsocket/IXUuid.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocket.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketCloseConstants.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketHandshake.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketHttpHeaders.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketPerMessageDeflate.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketPerMessageDeflateCodec.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketPerMessageDeflateOptions.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketProxyServer.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketServer.cpp
        NativeLib/dependencies/ixwebsocket/IXWebSocketTransport.cpp
        NativeLib/environment/libraries/debug.cpp
        NativeLib/environment/libraries/reflection.cpp
        NativeLib/environment/libraries/websocket.cpp
        NativeLib/environment/libraries/mthooks.cpp)

# Searches for a specified prebuilt library and stores the path as a
# variable. Because CMake includes system libraries in the search path by
# default, you only need to specify the name of the public NDK library
# you want to add. CMake verifies that the library exists before
# completing its build.

find_library( # Sets the name of the path variable.
        log-lib

        # Specifies the name of the NDK library that
        # you want CMake to locate.
        log)
find_package(Dobby REQUIRED CONFIG)

include_directories(prefab/modules/dobby/include)

# Specifies libraries CMake should link to your target library. You
# can link multiple libraries, such as libraries you define in this
# build script, prebuilt third-party libraries, or system libraries.
target_link_libraries( # Specifies the target library.
        mobileblox
        dobby::dobby

        # Links the target library to the log library
        # included in the NDK.
        ${log-lib})