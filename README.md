# DIKWP-MATH86 NATIVE81 ZERO-PRELOAD ATLAS v3.0.0

## Scope

This release does not merely rename and reorder conventional mathematical conjectures. The 86 conventional entries are demoted to an optional alias layer. The native core consists of 86 stable NIDs, five D/I/K/W/P positions, and all 25 directed position paths.

The core contains no conventional problem names, solved/unsolved labels, proof/counterexample verdicts, discipline labels, or final infinity object. Such material is retained only in `data/aliases.json` and source records for navigation and historical comparison. The dashboard starts in core-only mode and hides conventional aliases by default.

## Run

Open the following file in any modern browser:

```text
OPEN_DASHBOARD.html
```

It is a self-contained offline application with no server, network, or external JavaScript dependency.

## Validate the native core

```bash
python src/validate_native81.py --base . --out qa/native_validation_rerun.json
```

The validator checks the exact N001–N086 identity sequence, D/I/K/W/P-only core structure, all 25 paths, one-to-one alias mapping, the D81M carrier, deterministic digests, and the explicit absence of a terminal infinity object in the continuation demonstration.

## Browser smoke test

Python Playwright and Chromium are optional requirements:

```bash
python src/smoke_dashboard.py --html OPEN_DASHBOARD.html
```

The smoke test covers 86 cards, the 25-path matrix, core/alias switching, P>P filtering, two-record comparison, open integer continuation, and browser errors.

## Three-layer separation

1. **Native core** — `data/native_core.json` and `data/math86_native.d81m`. Only NIDs, D/I/K/W/P positions, paths, and opaque payloads have native runtime standing.
2. **Alias layer** — `data/aliases.json`. Conventional names, definition preloads, readable interpretations, and historical labels are optional and cannot govern the core.
3. **External history/source layer** — `data/references.json`. Public-history records remain available for communication without automatically rewriting native records.

## Boundary

This release reconstructs classification, carriers, and display authority. It does not claim that all 86 conventional external propositions have been proved or disproved. Conventional mathematical history is preserved, but it is not granted pre-native sovereignty over generation.

## License

Code, HTML, and structured data are released under Apache License 2.0. Third-party works cited or summarized in the report remain subject to their own rights and source terms.
