# Configuration file structure

Entity browsers are configuration entities that can be created [either by the site builder on the UI](creating_browser_through_ui.md) or imported from YAML configuration files.

If you are using a module that provides default or example configuration, these will be in the .yml files and will have the following structure (example ``` entity_browser.browser.field_files.yml``` from the example sub-module): 


```yaml
name: test_files
label: 'Test entity browser for files'
display: iframe
display_configuration:
  width: 650
  height: 500
  link_text: 'Select entities'
selection_display: no_display
selection_display_configuration: {  }
widget_selector: tabs
widget_selector_configuration: {  }
widgets:
  a4ad947c-9669-497c-9988-24351955a02f:
    settings:
      view: files_entity_browser
      view_display: entity_browser_1
    uuid: a4ad947c-9669-497c-9988-24351955a02f
    weight: 1
    label: 'Files listing'
    id: view
  735d146c-a4b2-4327-a057-d109e0905e05:
    settings:
      upload_location: 'public://'
    uuid: 735d146c-a4b2-4327-a057-d109e0905e05
    weight: 0
    label: 'Upload files'
    id: upload

```

The above configuration defines an entity browser that:
- is displayed in an iFrame 650px by 500px in size, 
- is displayed when the user clicks on "Select entities" link, 
- has no selection display,
- displays widgets as tabs,
- comes with two widgets:
  - a "file upload" widget that uploads files in the public:// directory,
  - a "view" browsing/selection widget that uses the display "entity_browser_1" of the view  "files_entity_browser".


- **name:** Unique machine name.
- **label:** Human readable name.
- **display:** ID of display plugin to be used.
- **display_configuration:** Display specific configuration. Depends on the display plugin used. See schema definitions provided by individual plugins (grep for "entity_browser.browser.display.*" in configuration schema yaml files).
- **selection_display:** ID of selection display plugin to be used.
- **selection_display_configuration:** Selection display specific configuration. Depends on the selection display plugin used. See schema definitions provided by individual plugins (grep for "entity_browser.browser.selection_display.*" in configuration schema yaml files).
- **widget_selector:** ID of widget selector plugin to be used.
- **widget_selector_configuration:** Widget selector specific configuration. Depends on the widget selector plugin used. See schema definitions provided by individual plugins (grep for "entity_browser.browser.widget_selector.*" in configuration schema yaml files).
- **widgets**: List of widgets to be used (keyed by UUID). Structure of individual entry:
  - **id:** ID of widget plugin.
  - **label:** Human readable name.
  - **weight:** Weight. Widgets are ordered ascending by wight.
  - **uuid:** Unique widget UUID. Must match the key.
  - **settings:** Widget specific configuration. Depends on the widget plugin used. See schema definitions provided by individual plugins (grep for "entity_browser.browser.widget.*" in configuration schema yaml files).
