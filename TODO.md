# TODO — Site issues & cleanup

Track issues found in the static portfolio site. Check off as they're fixed, one at a time.

## Content / accuracy
- [x] Update `<meta name="description">` — removed outdated ChargePoint mention.
- [x] Make profile image `alt` text descriptive (`alt="Portrait photo of Lukas Machegger"`).

## Accessibility
- [ ] Add `lang="en"` to the `<html>` element.
- [ ] Remove `user-scalable=no` from the viewport meta (allow pinch-to-zoom).
- [ ] Add `prefers-reduced-motion` handling for the slide-in animations.
- [ ] Review color contrast and focus states for keyboard navigation.

## SEO / metadata
- [ ] Add Open Graph / Twitter Card metadata for better link previews.
- [ ] Add a favicon (browsers currently hit `/favicon.ico` → 404).
- [ ] (Optional) Add `robots.txt` and a basic sitemap.

## Security / links
- [ ] Add `rel="noopener noreferrer"` to `target="_blank"` links.
- [ ] Remove `target="_blank"` from `mailto:` links (avoids stray blank tab).

## CSS / layout
- [ ] Replace `body { width: 100vw; }` with `100%` (or `overflow-x: hidden`) to avoid horizontal scroll from the scrollbar.
- [ ] Revisit `body { height: 100dvh; }` so taller content can scroll naturally.
- [ ] Remove dead CSS rule `#chargepoint-link` (no matching element).
- [ ] (Optional) Drop obsolete IE vendor prefixes (`-ms-interpolation-mode`, `-o-border-radius`, etc.).

## Assets / performance
- [ ] Serve an appropriately sized profile image (use `profile200.jpg` or add `srcset`) for the 100×100 display size.
- [ ] (Optional) Add image dimensions/aspect-ratio hints to reduce layout shift.

## Housekeeping
- [ ] Verify the custom domain/CNAME (`machegger.tech`) still resolves and SSL is valid.
- [ ] Consider splitting the single `index.html` copy for any future content updates.