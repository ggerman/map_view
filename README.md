# map_view

Server-side maps for Ruby on Rails.

Render maps directly from your Rails views using a single line of code.
No JavaScript required.

<%= map_for @locations %>

---

## What is map_view?

map_view is a Ruby on Rails helper that generates maps on the server side,
based on application data.

It is designed for backend-driven systems that need predictable, testable,
and deterministic map rendering.

The output is an image (PNG, JPG, or GIF), suitable for dashboards, reports,
exports, and internal tools.

---

## Who is this for?

- Ruby on Rails applications
- Admin panels and back-office systems
- Reports, PDFs, emails, and exports
- Legacy Rails apps with minimal frontend JavaScript
- Teams that prefer backend control and stability

---

## Why server-side maps?

Most mapping solutions rely on heavy frontend JavaScript and external APIs.

map_view takes a different approach:

- Maps are rendered on the server
- Output is a static image
- No client-side dependencies
- Easy to cache and test
- Predictable results

---

## Basic usage

In a Rails view:

<%= map_for @locations %>

With options:

<%= map_for @routes, zoom: 13 %>
<%= map_for @points, style: :dark %>
<%= map_for @track, animate: true %>

---

## Status

Early development.
APIs may change.

---

## License

See LICENSE file.
