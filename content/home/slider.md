+++
# Slider widget.
widget = "slider"  # See https://sourcethemes.com/academic/docs/page-builder/
headless = true  # This file represents a page section.
active = true  # Activate this widget? true/false
weight = 1  # Order that this section will appear.

# Slide interval.
# Use `false` to disable animation or enter a time in ms, e.g. `5000` (5s).
interval = false

# Minimum slide height.
# Specify a height to ensure a consistent height for each slide.
height = "500px"

# Slides.
# Duplicate an `[[item]]` block to add more slides.
[[item]]
  title = "Hello"
  content = ":heart:"
  align = "center"  # Choose `center`, `left`, or `right`.

  # Overlay a color or image (optional).
  #   Deactivate an option by commenting out the line, prefixing it with `#`.
  overlay_color = "#666"  # An HTML color value.
  overlay_img = "headers/Stanford_University_Aerial_View.jpg"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.5  # Darken the image. Value in range 0-1.

  # Call to action button (optional).
  #   Activate the button by specifying a URL and button label below.
  #   Deactivate by commenting out parameters, prefixing lines with `#`.
  # cta_label = "Get Academic"
  # cta_url = "https://sourcethemes.com/academic/"
  # cta_icon_pack = "fas"
  # cta_icon = "graduation-cap"

[[item]]
  title = ""
  content = ""
  align = "center"

  overlay_color = "#555"  # An HTML color value.
  overlay_img = "headers/Myschoollife.jpg"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.5  # Darken the image. Value in range 0-1.

[[item]]
  title = "Climbing"
  content = "Ap Lei Chau, Hong Kong :purple_heart:"
  align = "right"

  overlay_color = "#333"  # An HTML color value.
  overlay_img = "headers/Climbing.jpeg"  # Image path relative to your `static/img/` folder.
  overlay_filter = 0.4  # Darken the image. Value in range 0-1.
+++
