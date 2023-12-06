---

database-plugin: basic

---

```yaml:dbfolder
name: new database
description: new description
columns:
  __file__:
    key: __file__
    id: __file__
    input: markdown
    label: File
    accessorKey: __file__
    isMetadata: true
    skipPersist: false
    isDragDisabled: false
    csvCandidate: true
    position: 0
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: true
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  areas-of-concern:
    input: text
    accessorKey: areas-of-concern
    key: areas-of-concern
    id: areas-of-concern
    label: areas-of-concern
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  realm:
    input: text
    accessorKey: realm
    key: realm
    id: realm
    label: realm
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  adjective:
    input: text
    accessorKey: adjective
    key: adjective
    id: adjective
    label: adjective
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  symbol:
    input: text
    accessorKey: symbol
    key: symbol
    id: symbol
    label: symbol
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  alignment:
    input: select
    accessorKey: alignment
    key: alignment
    id: alignment
    label: alignment
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 122
    options:
      - { label: "Chaotic Good", value: "Chaotic Good", color: "hsl(107,93%,88%)"}
      - { label: "Neutral Good", value: "Neutral Good", color: "hsl(64,93%,88%)"}
      - { label: "Lawful Good", value: "Lawful Good", color: "hsl(152,93%,88%)"}
      - { label: "Chaotic Neutral", value: "Chaotic Neutral", color: "hsl(55, 95%, 90%)"}
      - { label: "Chaotic Evil", value: "Chaotic Evil", color: "hsl(0,93%,88%)"}
      - { label: "Lawful Evil", value: "Lawful Evil", color: "hsl(305,93%,88%)"}
      - { label: "Neutral Evil", value: "Neutral Evil", color: "hsl(267,93%,88%)"}
      - { label: "Lawful Neutral", value: "Lawful Neutral", color: "hsl(206,93%,88%)"}
      - { label: "True Neutral", value: "True Neutral", color: "hsl(237,93%,88%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
      option_source: manual
config:
  remove_field_when_delete_column: false
  cell_size: wide
  sticky_first_column: false
  group_folder_column: 
  remove_empty_folders: false
  automatically_group_files: false
  hoist_files_with_empty_attributes: true
  show_metadata_created: false
  show_metadata_modified: false
  show_metadata_tasks: false
  show_metadata_inlinks: false
  show_metadata_outlinks: false
  show_metadata_tags: false
  source_data: current_folder
  source_form_result: 
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 10
  font_size: 16
  enable_js_formulas: false
  formula_folder_path: /
  inline_default: false
  inline_new_position: last_field
  date_format: yyyy-MM-dd
  datetime_format: "yyyy-MM-dd HH:mm:ss"
  metadata_date_format: "yyyy-MM-dd HH:mm:ss"
  enable_footer: false
  implementation: default
filters:
  enabled: false
  conditions:
```