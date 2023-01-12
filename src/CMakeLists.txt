add_executable(qtTest main.cpp resources.qrc)
target_link_libraries(
qtTest Qt5::Quick Qt5::Qml Qt5::Gui Qt5::QuickControls2 Qt5::Widgets KF5::Kirigami2 KF5::I18n Qt5::Svg
)
if (ANDROID)
    find_package(Qt${QT_MAJOR_VERSION} ${QT_MIN_VERSION} REQUIRED COMPONENTS Svg)
    find_package(KF5 ${KF5_MIN_VERSION} REQUIRED COMPONENTS Kirigami2)
endif()
