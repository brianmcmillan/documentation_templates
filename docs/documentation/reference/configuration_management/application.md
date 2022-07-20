---
title: Application settings
---
<!---
Document the current project application settings.

File name: docs/configuration_management/software_bom.md
--->

### Datasette application settings
```json title="settings.json.txt"
{
    "default_page_size": 1000,
    "sql_time_limit_ms": 5000,
    "max_returned_rows": 5000,
    "num_sql_threads": 3,
    "allow_facet": true,
    "default_facet_size": 10,
    "facet_time_limit_ms": 1000,
    "facet_suggest_time_limit_ms": 500,
    "suggest_facets": true,
    "allow_download": true,
    "default_cache_ttl": 5,
    "default_cache_ttl_hashed": 31536000,
    "cache_size_kb": 0,
    "allow_csv_stream": true,
    "max_csv_mb": 0,
    "truncate_cells_html": 2048,
    "force_https_urls": false,
    "hash_urls": false,
    "template_debug": false,
    "base_url": "/"
}
```

### MkDocs
```yaml title="mkdocs.yml"
site_name: Data Product Documentation
site_url: https://example.com/
theme: 
name: material
palette: 
    - scheme: default
    primary: deep orange
    accent: indigo
    toggle:
        icon: material/toggle-switch 
        name: Switch to dark mode
    - scheme: slate 
    primary: deep purple
    toggle:
        icon: material/toggle-switch-off-outline
        name: Switch to light mode
features:
    - navigation.tabs  
    - navigation.tabs.sticky
    - navigation.expand
    - navigation.indexes
icon:
    logo: material/map 
plugins:
- search:
    lang: en  
- charts:
    vega_theme: default
    vega_renderer: "canvas"
- table-reader    
markdown_extensions:
- meta
- tables
- admonition
- pymdownx.details
- pymdownx.keys
- pymdownx.inlinehilite
- pymdownx.snippets:
    base_path: 'docs/'
- pymdownx.tasklist:
    custom_checkbox: true
- pymdownx.highlight:
    anchor_linenums: true
    linenums: true  
- pymdownx.tabbed:
    alternate_style: true 
- pymdownx.superfences:
    custom_fences:
        - name: mermaid
        class: mermaid
        format: !!python/name:pymdownx.superfences.fence_code_format
        - name: vegalite
        class: vegalite
        vega_theme: dark
        format: !!python/name:mkdocs_charts_plugin.fences.fence_vegalite
extra_javascript:
- https://unpkg.com/tablesort@5.3.0/dist/tablesort.min.js
- javascripts/tablesort.js          
- https://cdn.jsdelivr.net/npm/vega@5
- https://cdn.jsdelivr.net/npm/vega-lite@5
- https://cdn.jsdelivr.net/npm/vega-embed@6
```

