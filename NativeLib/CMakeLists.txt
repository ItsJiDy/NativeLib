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
        utils/utils.cpp
        roblox/hooks.cpp
        main.cpp
        exploit.cpp
        dependencies/luau/Ast/src/Ast.cpp
        dependencies/luau/Ast/src/Confusables.cpp
        dependencies/luau/Ast/src/Lexer.cpp
        dependencies/luau/Ast/src/Location.cpp
        dependencies/luau/Ast/src/Parser.cpp
        dependencies/luau/Ast/src/StringUtils.cpp
        dependencies/luau/Ast/src/TimeTrace.cpp
        dependencies/luau/Compiler/src/BuiltinFolding.cpp
        dependencies/luau/Compiler/src/Builtins.cpp
        dependencies/luau/Compiler/src/BytecodeBuilder.cpp
        dependencies/luau/Compiler/src/Compiler.cpp
        dependencies/luau/Compiler/src/ConstantFolding.cpp
        dependencies/luau/Compiler/src/CostModel.cpp
        dependencies/luau/Compiler/src/lcode.cpp
        dependencies/luau/Compiler/src/TableShape.cpp
        dependencies/luau/Compiler/src/Types.cpp
        dependencies/luau/Compiler/src/ValueTracking.cpp
        dependencies/luau/VM/src/lapi.cpp
        dependencies/luau/VM/src/laux.cpp
        dependencies/luau/VM/src/lbaselib.cpp
        dependencies/luau/VM/src/lbitlib.cpp
        dependencies/luau/VM/src/lbuiltins.cpp
        dependencies/luau/VM/src/lcorolib.cpp
        dependencies/luau/VM/src/ldblib.cpp
        dependencies/luau/VM/src/ldebug.cpp
        dependencies/luau/VM/src/ldo.cpp
        dependencies/luau/VM/src/lfunc.cpp
        dependencies/luau/VM/src/lgc.cpp
        dependencies/luau/VM/src/lgcdebug.cpp
        dependencies/luau/VM/src/linit.cpp
        dependencies/luau/VM/src/lmathlib.cpp
        dependencies/luau/VM/src/lmem.cpp
        dependencies/luau/VM/src/lnumprint.cpp
        dependencies/luau/VM/src/lobject.cpp
        dependencies/luau/VM/src/loslib.cpp
        dependencies/luau/VM/src/lperf.cpp
        dependencies/luau/VM/src/lstate.cpp
        dependencies/luau/VM/src/lstring.cpp
        dependencies/luau/VM/src/lstrlib.cpp
        dependencies/luau/VM/src/ltable.cpp
        dependencies/luau/VM/src/ltablib.cpp
        dependencies/luau/VM/src/ltm.cpp
        dependencies/luau/VM/src/ludata.cpp
        dependencies/luau/VM/src/lutf8lib.cpp
        dependencies/luau/VM/src/lvmexecute.cpp
        dependencies/luau/VM/src/lvmload.cpp
        dependencies/luau/VM/src/lvmutils.cpp
        roblox/update.cpp
        execution/execution.cpp
        environment/libraries/misc.cpp
        environment/environment.cpp
        taskscheduler/taskscheduler.cpp
        callcheck/callcheck.cpp
        dependencies/cpr/auth.cpp
        dependencies/cpr/cookies.cpp
        dependencies/cpr/cprtypes.cpp
        dependencies/cpr/digest.cpp
        dependencies/cpr/error.cpp
        dependencies/cpr/multipart.cpp
        dependencies/cpr/parameters.cpp
        dependencies/cpr/payload.cpp
        dependencies/cpr/proxies.cpp
        dependencies/cpr/session.cpp
        dependencies/cpr/ssl_options.cpp
        dependencies/cpr/timeout.cpp
        dependencies/cpr/util.cpp
        dependencies/imgui/backends/imgui_impl_android.cpp
        dependencies/imgui/backends/imgui_impl_opengl3.cpp
        dependencies/imgui/imgui.cpp
        dependencies/imgui/imgui_demo.cpp
        dependencies/imgui/imgui_draw.cpp
        dependencies/imgui/imgui_tables.cpp
        dependencies/imgui/imgui_widgets.cpp
        dependencies/luau/VM/src/lbuffer.cpp
        dependencies/luau/VM/src/lbuflib.cpp
        dependencies/lz4/lz4.cpp
        environment/libraries/closure.cpp
        reflection/instance.cpp
        renderer/renderer.cpp
        dependencies/ixwebsocket/IXBench.cpp
        dependencies/ixwebsocket/IXCancellationRequest.cpp
        dependencies/ixwebsocket/IXConnectionState.cpp
        dependencies/ixwebsocket/IXDNSLookup.cpp
        dependencies/ixwebsocket/IXExponentialBackoff.cpp
        dependencies/ixwebsocket/IXGetFreePort.cpp
        dependencies/ixwebsocket/IXGzipCodec.cpp
        dependencies/ixwebsocket/IXHttp.cpp
        dependencies/ixwebsocket/IXHttpClient.cpp
        dependencies/ixwebsocket/IXHttpServer.cpp
        dependencies/ixwebsocket/IXNetSystem.cpp
        dependencies/ixwebsocket/IXSelectInterrupt.cpp
        dependencies/ixwebsocket/IXSelectInterruptEvent.cpp
        dependencies/ixwebsocket/IXSelectInterruptFactory.cpp
        dependencies/ixwebsocket/IXSelectInterruptPipe.cpp
        dependencies/ixwebsocket/IXSetThreadName.cpp
        dependencies/ixwebsocket/IXSocket.cpp
        dependencies/ixwebsocket/IXSocketAppleSSL.cpp
        dependencies/ixwebsocket/IXSocketConnect.cpp
        dependencies/ixwebsocket/IXSocketFactory.cpp
        dependencies/ixwebsocket/IXSocketMbedTLS.cpp
        dependencies/ixwebsocket/IXSocketOpenSSL.cpp
        dependencies/ixwebsocket/IXSocketServer.cpp
        dependencies/ixwebsocket/IXSocketTLSOptions.cpp
        dependencies/ixwebsocket/IXStrCaseCompare.cpp
        dependencies/ixwebsocket/IXUdpSocket.cpp
        dependencies/ixwebsocket/IXUrlParser.cpp
        dependencies/ixwebsocket/IXUserAgent.cpp
        dependencies/ixwebsocket/IXUuid.cpp
        dependencies/ixwebsocket/IXWebSocket.cpp
        dependencies/ixwebsocket/IXWebSocketCloseConstants.cpp
        dependencies/ixwebsocket/IXWebSocketHandshake.cpp
        dependencies/ixwebsocket/IXWebSocketHttpHeaders.cpp
        dependencies/ixwebsocket/IXWebSocketPerMessageDeflate.cpp
        dependencies/ixwebsocket/IXWebSocketPerMessageDeflateCodec.cpp
        dependencies/ixwebsocket/IXWebSocketPerMessageDeflateOptions.cpp
        dependencies/ixwebsocket/IXWebSocketProxyServer.cpp
        dependencies/ixwebsocket/IXWebSocketServer.cpp
        dependencies/ixwebsocket/IXWebSocketTransport.cpp
        environment/libraries/debug.cpp
        environment/libraries/reflection.cpp
        environment/libraries/websocket.cpp
        environment/libraries/mthooks.cpp)

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