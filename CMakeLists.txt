# ImGui Submodule Project
add_library(ImGui imconfig.h
		imgui.h
		imgui.cpp
		imgui_draw.cpp
		imgui_tables.cpp
		imgui_internal.h
		imgui_widgets.cpp
		imstb_rectpack.h
		imstb_textedit.h
		imstb_truetype.h
		imgui_demo.cpp	
	)

if(CMAKE_BUILD_TYPE STREQUAL "Release")
    target_compile_definitions(ImGui
            PUBLIC NDEBUG=1
        )
endif()
