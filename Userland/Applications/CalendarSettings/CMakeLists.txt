serenity_component(
    CalendarSettings
    RECOMMENDED
    TARGETS CalendarSettings
)

compile_gml(CalendarSettingsWidget.gml CalendarSettingsWidgetGML.h calendar_settings_widget_gml)

set(SOURCES
    main.cpp
    CalendarSettingsWidget.cpp
    CalendarSettingsWidget.h
    CalendarSettingsWidgetGML.h
)

serenity_app(CalendarSettings ICON app-calendar)
target_link_libraries(CalendarSettings LibConfig LibGUI LibMain)
