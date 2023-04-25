---
id: 'Test demo'
beta: true
section: patterns
cssPrefix: pf-v5-d-test-demo
---

import "./test-demo.css"

## Examples
### new
```hbs isFullscreen
{{> page-template
      page-template--id="page-demo-centered-section"
}}

{{#*inline "page-template-main-content"}}
  {{#> page-main-section page-main-section--IsLimitWidth="true" page-main-section--modifier="pf-  m-align-center pf-m-light"}}
    {{#> test-demo}}
      Update Basic example content
      <div class="pf-c-card">
        <div class="pf-c-card__header">
          test header
        </div>
        <div class="pf-c-card__body">
          test body
        </div>
      </div>

      {{#> card card--version='pf-c-sss'}}
        {{#> card-title}}
          Header
        {{/card-title}}
      {{/card}}
    {{/test-demo}}
    {{> card-template-gallery card-template-gallery--id="card-view-basic-example-gallery"}}

  {{/page-main-section}}
{{/inline}}
```

### Basic
```hbs isFullscreen
{{#> test-demo}}
  Basic example content
  <div class="pf-c-card">
    <div class="pf-c-card__header">
      test header
    </div>
    <div class="pf-c-card__body">
      test body
    </div>
  </div>
  {{#> card}}
    {{#> card-header}}
      Header
    {{/card-header}}
  {{/card}}
{{/test-demo}}
```

## Documentation
