+++
widget = "portfolio"  # Use the Portfolio widget
headless = true  # This file represents a page section.
active = false
weight = 30

# ... Put Your Section Options Here (title etc.) ...
title = "Projects"

[content]
  # Page type to display. E.g. project.
  page_type = "project"
  
  # Filter toolbar (optional).
  # Add or remove as many filters (`[[content.filter_button]]` instances) as you like.
  # To show all items, set `tag` to "*".
  # To filter by a specific tag, set `tag` to an existing tag name.
  # To remove toolbar, delete/comment all instances of `[[content.filter_button]]` below.
  
  # Default filter index (e.g. 0 corresponds to the first `[[filter_button]]` instance below).
  # filter_default = 0
  
  # [[content.filter_button]]
  #  name = "All"
  #  tag = "*"
  
  # [[content.filter_button]]
  #  name = "Deep Learning"
  #  tag = "Deep Learning"
  
  # [[content.filter_button]]
  #  name = "Other"
  #  tag = "Demo"

[design]
  # Choose how many columns the section has. Valid values: 1 or 2.
  columns = "2"

  # Toggle between the various page layout types.
  #   1 = List
  #   2 = Compact  
  #   3 = Card
  #   5 = Showcase
  view = 3

  # For Showcase view, flip alternate rows?
  flip_alt_rows = false
+++
