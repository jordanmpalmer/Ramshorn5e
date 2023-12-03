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
    position: 1
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
      wrap_content: false
  tags:
    input: tags
    accessorKey: tags
    key: tags
    id: tags
    label: tags
    position: 9
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "[,NPC]", value: "[,NPC]", color: "hsl(298, 95%, 90%)"}
      - { label: "[,PC_NPC]", value: "[,PC_NPC]", color: "hsl(89, 95%, 90%)"}
      - { label: "[,,NPC]", value: "[,,NPC]", color: "hsl(266, 95%, 90%)"}
      - { label: "[,,PC_NPC]", value: "[,,PC_NPC]", color: "hsl(286, 95%, 90%)"}
      - { label: "[NPC]", value: "[NPC]", color: "hsl(156, 95%, 90%)"}
      - { label: "[PC_NPC]", value: "[PC_NPC]", color: "hsl(268, 95%, 90%)"}
      - { label: "NPC", value: "NPC", color: "hsl(273, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  aliases:
    input: text
    accessorKey: aliases
    key: aliases
    id: aliases
    label: aliases
    position: 2
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 115
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  group:
    input: select
    accessorKey: group
    key: group
    id: group
    label: group
    position: 4
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 167
    options:
      - { label: "The Magebreaker Initiative", value: "The Magebreaker Initiative", color: "hsl(343, 95%, 90%)"}
      - { label: "Cult of the Choir", value: "[[Cult of the Choir]]", color: "hsl(201, 95%, 90%)"}
      - { label: "The Empire", value: "[[The Empire]]", color: "hsl(187, 95%, 90%)"}
      - { label: "The Reclaimers", value: "[[The Reclaimers]]", color: "hsl(321, 95%, 90%)"}
      - { label: "The Sheperds", value: "[[The Sheperds]]", color: "hsl(55, 95%, 90%)"}
      - { label: "[[3. Background/Guilds and Groups/The Reclaimers.md|The Reclaimers]]", value: "[[3. Background/Guilds and Groups/The Reclaimers.md|The Reclaimers]]", color: "hsl(310, 95%, 90%)"}
      - { label: "Name of Guild or Group they belong to", value: "Name of Guild or Group they belong to", color: "hsl(17, 95%, 90%)"}
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
  sex:
    input: select
    accessorKey: sex
    key: sex
    id: sex
    label: sex
    position: 8
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 70
    options:
      - { label: "Male", value: "Male", color: "hsl(308, 95%, 90%)"}
      - { label: "Female", value: "Female", color: "hsl(81, 95%, 90%)"}
      - { label: "Male or Female or...", value: "Male or Female or...", color: "hsl(352, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  race:
    input: select
    accessorKey: race
    key: race
    id: race
    label: race
    position: 6
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Dragon", value: "Dragon", color: "hsl(46, 95%, 90%)"}
      - { label: "Human, Dwarf, Elf, etc", value: "Human, Dwarf, Elf, etc", color: "hsl(325, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  class:
    input: select
    accessorKey: class
    key: class
    id: class
    label: class
    position: 7
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Warrior, Wizard, Rogue, etc", value: "Warrior, Wizard, Rogue, etc", color: "hsl(132, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  party-alignment:
    input: select
    accessorKey: party-alignment
    key: party-alignment
    id: party-alignment
    label: party-alignment
    position: 3
    skipPersist: false
    isHidden: false
    sortIndex: -1
    width: 83
    options:
      - { label: "Friend", value: "Friend", color: "hsl(20, 95%, 90%)"}
      - { label: "Foe", value: "Foe", color: "hsl(79, 95%, 90%)"}
      - { label: "Neutral", value: "Neutral", color: "hsl(54, 95%, 90%)"}
      - { label: "Unknown", value: "Unknown", color: "hsl(307, 95%, 90%)"}
      - { label: "friend or foe?", value: "friend or foe?", color: "hsl(98, 95%, 90%)"}
    config:
      enable_media_view: true
      link_alias_enabled: true
      media_width: 100
      media_height: 100
      isInline: false
      task_hide_completed: true
      footer_type: none
      persist_changes: false
  location:
    input: select
    accessorKey: location
    key: location
    id: location
    label: location
    position: 5
    skipPersist: false
    isHidden: false
    sortIndex: -1
    options:
      - { label: "Minastria", value: "[[Minastria]]", color: "hsl(154, 95%, 90%)"}
      - { label: "Mirage-Oasis", value: "[[Mirage Oasis]]", color: "hsl(151, 95%, 90%)"}
      - { label: "Ramshorn", value: "[[Ramshorn]]", color: "hsl(97, 95%, 90%)"}
      - { label: "Regatia", value: "[[Regatia]]", color: "hsl(41, 95%, 90%)"}
      - { label: "[[3. Background/Places/Minastria.md|Minastria]]", value: "[[3. Background/Places/Minastria.md|Minastria]]", color: "hsl(164, 95%, 90%)"}
      - { label: "[[3. Background/Places/Regatia.md|Regatia]]", value: "[[3. Background/Places/Regatia.md|Regatia]]", color: "hsl(236, 95%, 90%)"}
      - { label: "[[3. Background/Places/Ramshorn.md|Ramshorn]]", value: "[[3. Background/Places/Ramshorn.md|Ramshorn]]", color: "hsl(59, 95%, 90%)"}
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
  source_data: tag
  source_form_result: "#NPC"
  source_destination_path: /
  row_templates_folder: /
  current_row_template: 
  pagination_size: 50
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