# SVG authoring and visual QA

Read this reference whenever producing or revising the final SVG.

## Composition

- Establish a strong hierarchy: title, shared system, process, examples or lanes, feedback, enabling layer, footer.
- Keep the dominant reading direction top-to-bottom for portrait maps.
- Use alignment and whitespace before adding boxes or dividers.
- Limit the main palette to one neutral family plus semantic accents.
- Preserve source-highlight meaning; never reuse the same accent for an unrelated concept.

## Geometry

- Use a stable viewBox and avoid transforms that make later editing unnecessarily difficult.
- Keep outer margins at roughly 6–8% of canvas width.
- Use consistent radii, padding, border weights, and connector styles.
- Route connectors around text. Use arrowheads consistently and distinguish sequence from feedback with line style or color.
- Leave at least one text-line height between independent groups.

## Typography

- Use language-appropriate fallback stacks, such as `"Noto Sans TC", "Microsoft JhengHei", "PingFang TC", sans-serif` for Traditional Chinese.
- Define text styles in `<style>` rather than repeating attributes.
- Use no more than four type scales in the main diagram.
- Manually wrap long text using separate `<text>` or `<tspan>` lines; do not rely on browser-specific wrapping.
- Avoid labels below 15 px on a 1200 × 1800 canvas.

## Technical quality

- Include `xmlns`, `viewBox`, `role="img"`, `<title>`, and `<desc>`.
- Give definitions unique IDs and ensure every `url(#id)` reference resolves.
- Keep effects modest; strong blurs can crop or render inconsistently.
- Avoid external assets, external fonts, scripts, and network dependencies.
- Prefer vector icons constructed from basic paths and shapes.
- Keep opacity and contrast suitable for both screen viewing and export.

## Content QA

Check the final map against the confirmed semantic model:

- all required entities are present;
- examples are not mistaken for universal stages;
- process order matches the user's intent;
- percentages and metrics have the right scope;
- feedback loops return to the correct stage;
- legends explain semantic colors when color meaning is not obvious;
- uncertain text is omitted, marked, or disclosed rather than invented.

## Revision QA

After a correction, trace downstream effects. A changed entity may require updates to its lane, connector, legend, metric, accessibility description, and footer summary. Recheck the whole diagram, not just the edited label.
