cmake_minimum_required(VERSION 3.5)

project(nuklear-examples-vcpkg)

find_package(GLEW REQUIRED)
find_package(glfw3 REQUIRED)
find_package(opengl REQUIRED)

add_executable(nuklear-canvas canvas.c)
add_executable(nuklear-extended extended.c)
add_executable(nuklear-file_browser file_browser.c getopt.c)
add_executable(nuklear-skinning skinning.c)

target_link_libraries(nuklear-canvas PRIVATE 
	glfw
	GLEW::GLEW
	opengl32
	)

target_link_libraries(nuklear-extended PRIVATE 
	glfw
	GLEW::GLEW
	opengl32
	)

target_link_libraries(nuklear-file_browser PRIVATE 
	glfw
	GLEW::GLEW
	opengl32
	)

target_link_libraries(nuklear-skinning PRIVATE 
	glfw
	GLEW::GLEW
	opengl32
	)

file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/skins/gwen.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/skins)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image1.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image2.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image3.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image4.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image5.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image6.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image7.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image8.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/images/image9.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/images)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/checked.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/cloud.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/computer.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/copy.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/default.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/delete.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/desktop.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/directory.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/edit.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/export.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/font.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/home.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/img.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/movie.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/music.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/next.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/pause.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/pen.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/phone.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/plane.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/play.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/prev.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/rocket.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/settings.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/stop.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/text.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/tools.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/unchecked.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/wifi.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/icon/volume.png DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/icon)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/Cousine-Regular.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/DroidSans.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/Karla-Regular.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/kenvector_future.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/kenvector_future_thin.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/ProggyClean.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/ProggyTiny.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/Raleway-Bold.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/Roboto-Bold.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/Roboto-Light.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)
file(COPY ${CMAKE_CURRENT_SOURCE_DIR}/extra_font/Roboto-Regular.ttf DESTINATION ${CMAKE_CURRENT_BINARY_DIR}/extra_font)