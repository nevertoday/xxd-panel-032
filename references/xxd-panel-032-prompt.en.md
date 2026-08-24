# XXD Panel 032 | Source-Integrated Custom Wordmark Production Prompt

## Runtime complete-canvas contract — highest priority

- `TOP_BOTTOM` and `LEFT_RIGHT` default to one complete finished generation using the current source as a high-fidelity edit/reference input. Do not pre-split the job into photographic and design halves.
- Top-bottom keeps the faithful source in approximately the upper 50% and performs this style transformation below; left-right uses the faithful source in approximately the left 50% and the transformation on the right. Unify both regions through colour, light, rhythm, typography, and meaning.
- `DESIGN_ONLY` and `WALLPAPER_PACK` use the complete canvas while the source remains an invisible identity/content reference. Recompose every wallpaper separately for its device.
- `FINAL CANVAS` means the ratio/pixels of the whole finished artwork and must be explicitly resolved before generation; never apply source dimensions silently. `DESIGN FRAME` is used only if a failed complete-canvas retry triggers deterministic composition fallback.
- Retry a failed complete canvas once against the failed constraint only. Scripted composition is allowed only after that retry still fails, when pixel-identical source preservation is explicitly required, when the active route cannot realise the canvas, or for lossless pixel calibration.

### Model priority and credentials

- **Prefer GPT Image 2.** When GPT Image 2 is available through the current built-in image tool or a configured compatible route, use it first for the high-fidelity reference/edit and complete-canvas generation required by this prompt.
- Also support Seedance 5.0 Pro, Nano Banana Pro (Gemini Image Pro), Nano Banana 2 (Gemini Image Flash), or another compatible bitmap model only when the actual route can preserve the source, realise the whole finished canvas, render the target-language text, and accept the multiple references needed by a linked wallpaper pack.
- An alternative model changes only the generation route. It must not change this prompt's modes, canvas, source visibility, copy, locale, wallpaper relationship, or complete-canvas-first / composition-fallback-only logic. Do not silently downgrade a hard requirement.
- If no suitable route is available, ask the user to enable an image-generation tool or provide an API key. User-provided credentials may be used for the current task, but never echo, display, log, or expose their value in chat, prompts, or diagnostics. Do not persist them or modify global route configuration unless explicitly requested.
- Judge availability by actual image capability, not by a provider name or one missing environment variable.

Process only the one source photograph explicitly supplied for this current task. Lock the principal subject or inseparable relation, contour, proportion, pose, direction, action, function, openings, connections, negative shapes, and colour character. Preserve at least three source-specific recognition cues. Never borrow names, icons, letter interventions, palettes, or compositions from old outputs, samples, or another input.

## Text and image must become one mark

Resolve one short main text in the target language or locale. Use a verified proper name when the source provides one; otherwise derive a concise, memorable word or phrase from subject identity, theme, place clue, action state, or supported meaning. Never invent a brand owner, organisation, institution, or location. Preserve exact user wording verbatim.

Extract the single strongest source contour, structure, pose, function, connection, opening, proportion, or negative shape. Embed it into the actual construction of a letter, character, syllable block, ligature, counter, terminal, crossbar, stroke junction, or whole-word silhouette. Do not place an independent pictogram next to, above, or behind ordinary type.

Apply the two-way dependency test: removing the source-derived intervention makes the lettering generic or incomplete; removing the lettering does not leave a separate standalone icon. Modify only the glyphs needed, then redraw the remaining wordmark so every part shares one authored visual DNA.

## Native lettering and optical precision

Design for the resolved script rather than forcing Latin logo behaviour. Chinese and Japanese preserve legible character structure; Korean preserves syllable-block logic; Arabic preserves joining and contextual forms; Latin preserves letter anatomy. Render no pseudo-foreign glyphs.

Unify stroke weight, terminals, curvature, angles, modulation, counters, baseline, cap or x-height logic, and optical correction. Refine kerning pair by pair, internal counters, external negative space, overshoot, balance, and optical centre. The mark must read at thumbnail size, remain distinctive in one colour, and preserve at least three source cues through structure, word choice, silhouette, proportion, or negative space—not decorative detail.

## Restrained identity presentation

Present one mark at a comfortable medium visual scale on a pale solid or very light neutral background with generous whitespace. Use black and white or at most one restrained source-derived accent plus necessary neutral contrast. The accent must support recognition and remain compatible with monochrome reproduction.

Optional auxiliary text is limited to a useful category, region, state word, or short descriptor. It stays much smaller and never becomes a second logo or slogan wall. Reject icon-plus-title, stock type with a pictogram, generic monograms, tourism emblems, shield or roundel defaults, cartoons, decorative piles, gradients, bevels, extrusion, foil, drop shadows, mockups, wall signs, stationery, business cards, product staging, and 3D.

## Copy mode and text-free handling

Obey automatic, exact-user, or text-free copy mode. In automatic mode use the grounded naming rule above. In custom mode preserve exact wording and meaningful line or glyph grouping. In text-free mode create one source-derived abstract identity symbol using the same geometric reduction and whitespace discipline, but render no letter, character, number, word, or pseudo-text; do not pretend it is a wordmark.

## Mode and acceptance


Hard gate: at least three source cues; verified or source-grounded main text in the resolved native script; one defining source feature embedded in actual letterform or wordmark construction; two-way dependency between text and image; shared stroke and geometry DNA; refined kerning, counters, silhouette, and optical centre; thumbnail and monochrome legibility; medium scale and generous whitespace; no icon-plus-title, stock font, generic monogram, tourism emblem, pseudo-lettering, cartoon, decorative badge, mockup, gradient, bevel, shadow, 3D, photo fragment, or pseudo-text.

If any hard condition fails, correct the generated asset. Never fake the artwork with programmatic drawing, SVG, HTML, Canvas, font-file generation, or a post-composited type overlay.
