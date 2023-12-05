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
  aliases:
    input: text
    accessorKey: aliases
    key: aliases
    id: aliases
    label: aliases
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
  locations:
    input: select
    accessorKey: locations
    key: locations
    id: locations
    label: locations
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Minastria", value: "[[Minastria]]", color: "hsl(34, 95%, 90%)"}
      - { label: "MirageOasis", value: "[[Mirage Oasis]]", color: "hsl(335, 95%, 90%)"}
      - { label: "Ramshorn", value: "[[Ramshorn]]", color: "hsl(217, 95%, 90%)"}
      - { label: "Regatia", value: "[[Regatia]]", color: "hsl(192, 95%, 90%)"}
      - { label: "[[3. Background/Places/Mirage Oasis.md|Mirage Oasis]]", value: "[[3. Background/Places/Mirage Oasis.md|Mirage Oasis]]", color: "hsl(278, 95%, 90%)"}
      - { label: "[[3. Background/Places/Minastria.md|Minastria]]", value: "[[3. Background/Places/Minastria.md|Minastria]]", color: "hsl(274, 95%, 90%)"}
      - { label: "[[3. Background/Places/Regatia.md|Regatia]]", value: "[[3. Background/Places/Regatia.md|Regatia]]", color: "hsl(144, 95%, 90%)"}
      - { label: "[[3. Background/Places/Ramshorn.md|Ramshorn]]", value: "[[3. Background/Places/Ramshorn.md|Ramshorn]]", color: "hsl(35, 95%, 90%)"}
      - { label: "[[3. World/Places/Minastria/Mirage Oasis.md|Mirage Oasis]]", value: "[[3. World/Places/Minastria/Mirage Oasis.md|Mirage Oasis]]", color: "hsl(44, 95%, 90%)"}
      - { label: "[[3. World/Places/Minastria/Minastria.md|Minastria]]", value: "[[3. World/Places/Minastria/Minastria.md|Minastria]]", color: "hsl(55, 95%, 90%)"}
      - { label: "[[3. World/Places/Agrevar/Regatia.md|Regatia]]", value: "[[3. World/Places/Agrevar/Regatia.md|Regatia]]", color: "hsl(194, 95%, 90%)"}
      - { label: "[[3. World/Places/Minastria/Ramshorn.md|Ramshorn]]", value: "[[3. World/Places/Minastria/Ramshorn.md|Ramshorn]]", color: "hsl(35, 95%, 90%)"}
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
  tags:
    input: tags
    accessorKey: tags
    key: tags
    id: tags
    label: tags
    position: 100
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "group", value: "group", color: "hsl(341, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
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