---
permalink: /utilities/clearfix/
layout: styleguide
type: utility
title: Clearfix
category: Utilities
lead: Clear any floated elements

subnav:
- text: Utility mixins
  href: '#utility-mixins'
- text: Advanced settings
  href: '#advanced-settings'

utilities:
- base:         clearfix
  var:          clearfix
  output:       true
  responsive:   false
  active:       false
  focus:        false
  hover:        false
  visited:      false
---

<section class="utilities-section">
  <div class="grid-row utilities-section-title-bar">
    <h2 class="grid-col-auto utilities-section-title">Examples and usage</h2>
    <p class="grid-col-fill utilities-section-helper">Utilities, values, and variants may be activated and deactivated in <a href="#advanced-settings" class="text-ink text-no-wrap">advanced settings</a>.</p>
  </div>

  <section class="utility" id="utility-clearfix">
    <section class="utility-title-bar">
      <div class="grid-row">
        <div class="grid-col-fill">
          <h3 class="grid-col-auto utility-title">Clearfix</h3>
        </div>
        <ul class="grid-col-auto utility-scope">
          <li class="utility-scope-button-disabled">responsive</li>
          <li class="utility-scope-button-disabled">active</li>
          <li class="utility-scope-button-disabled">hover</li>
          <li class="utility-scope-button-disabled">focus</li>
          <li class="utility-scope-button-disabled">visited</li>
        </ul>
      </div>
    </section><!-- .utility-title-bar -->

    <section class="utility-examples">
      <div class="clearfix border-1px">
        <span class="float-left bg-secondary-light padding-2">.float-left</span>
        <span class="float-right bg-secondary-light padding-2">.float-right</span>
      </div>
      <div class="usa-accordion-bordered usa-code-sample margin-top-4">
        <button class="usa-accordion-button" aria-controls="code-clearfix" aria-expanded="true">Code</button>
        <div id="code-clearfix" class="usa-accordion-content margin-bottom-1">
<div markdown="1">
```html
<div class="clearfix">
  <span class="float-left">.float-left</span>
  <span class="float-right">.float-right</span>
</div>
```
</div>
        </div>
      </div>
    </section><!-- .utility-examples -->
  </section><!-- .utility#clearfix -->
</section><!-- .utilities -->

<section class="utilities-section margin-top-6">
  <h2 class="utilities-section-title">Default output</h2>
  <table class="usa-table-borderless site-table-responsive site-table-simple">
    <thead>
      <tr>
        <th scope="col" class="tablet:maxw-card-lg">Utility</th>
        <th scope="col">Output</th>
      </tr>
    </thead>
    <tbody class="font-mono-2xs">
      <tr>
        <td scope="row" data-title="Utility" class="tablet:text-no-wrap tablet:maxw-card-lg">
          <span>
            .clearfix
          </span>
        </td>
        <td data-title="Output">
          <span>
            ::after { clear: both; content: ""; display: block; }
          </span>
        </td>
      </tr>
    </tbody>
  </table>
</section>

<section id="utility-mixins" class="padding-top-4">
  <h2 class="site-h2 margin-y-0">Utility mixins</h2>
  {% include utilities/utility-mixin-intro.html %}
  <table class="usa-table-borderless site-table-responsive site-table-simple">
    <thead>
      <tr>
        <th scope="col" class="tablet:maxw-card-lg">Utility</th>
        <th scope="col">Mixin</th>
        <th scope="col">Example</th>
      </tr>
    </thead>
    <tbody class="font-mono-2xs">
      <tr>
        <td scope="row" data-title="Utility" class="tablet:text-no-wrap tablet:maxw-card-lg">
          <span>
            .cleafix
          </span>
        </td>
        <td data-title="Mixin">
          <span>
            clearfix
          </span>
        </td>
        <td data-title="Example">
          <span>
            @include clearfix
          </span>
        </td>
      </tr>
    </tbody>
  </table>
  {% include utilities/utility-mixin-using.html %}
</section>

<section id="advanced-settings" class="padding-top-4">
<h2 class="site-h2 margin-y-0">Advanced settings</h2>

  {% include utilities/responsive-variants.html %}

  {% include utilities/state-variants.html %}

  {% include utilities/output-control.html %}

  {% include utilities/values-no-custom-values.html %}
</section>