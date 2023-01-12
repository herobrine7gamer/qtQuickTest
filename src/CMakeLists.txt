# SPDX-FileCopyrightText: 2023 HEROBRINE7GAMER <tapermeerkat77@gmail.com>
# SPDX-License-Identifier: GPL-3.0

add_executable(qtQuickTest
    main.cpp
    resources.qrc)

target_link_libraries(kontrast
    Qt::Core
    Qt::Gui
    Qt::Qml
    Qt::Quick
    Qt::QuickControls2
    Qt::Sql
    Qt::Svg
    KF5::I18n
    KF5::CoreAddons)
