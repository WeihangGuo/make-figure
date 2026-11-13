# Compact paper figures

Make the method easy to follow at the final display size. Empty space must
separate content, provide a route for a connection, or support a label.

## Arrange the content

- Start with the method and its connections. Keep the existing scientific facts.
- Use 24–32 SVG units between adjacent blocks as a starting point. A larger gap
  needs a purpose: a label, a branch, or a group boundary.
- Size blocks for their labels and insets. Do not make all blocks the same size.
- Place a side input close to its receiving module. Keep its route clear.
- For two towers, measure the full row, including tensor labels and side inputs.
  Start with 24–36 units between that row and the next. Check stack offsets too.
- For a matrix, place definitions and equations beside it. Align both columns
  near their top and bottom. Avoid a separate formula row under a short matrix
  when this leaves the other column empty.
- Keep 16–24 units at the outer edges when practical. Allow space for long
  labels, arrowheads and subscripts. Fit width and height after placing content.
- Place the legend close to the content. Use `legend_align: "center"` when a
  left-aligned legend leaves an unbalanced footer.

These values are starting points, not automatic acceptance limits. The renderer
uses explicit coordinates; it does not compact a figure or measure text for you.

## Inspect each pass

1. Render with Newsreader fully loaded. Check the image, not just the source.
2. Identify the largest empty region. State what it does. If it has no purpose,
   move nearby content or reduce the canvas. Do not add decorative content.
3. Keep labels readable. Shorten labels or change the layout before shrinking type.
4. Trace each input to its output. Check that lines reach the correct ports.
5. Check labels, subscripts, stack layers, legends and the canvas edges for overlap.
6. Compare with the previous pass. Record the change and its visible effect.
7. Stop when the empty regions have a purpose and further compression reduces
   readability. Preserve both rendered examples for the user to inspect.

Expose a mechanism from existing source material only when it helps explain the
method. Do not invent layers, tensors, numbers or results to fill an empty area.
