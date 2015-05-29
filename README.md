# MOJULAR

Bower-friendly MOJ template, styles and assets.

## Templates

Two variations of the same template are available:

- **external** for citizen facing services (this uses the GOV.UK logo)
- **internal** for non citizen staff applications

### To use

In a Ruby on Rails application, `applicaiton.html.erb`

```erb
<%= render template: 'layouts/erb/internal' %>
```

or alternatively in `application_controller.rb`

```ruby
layout 'erb/external'
```

### Content blocks

You can specify content for the following yield placeholders.

Yield                | Position
-------------------- | --------
`page_title`         | The whole `<title>` element
`header_content`     | Internal template only
`proposition`        | External template only. Nested within `header_content`.
`global_subheader`   | First element in main content
`support_links`      | Internal template only
`include_js`         | Last item in `<body>`
