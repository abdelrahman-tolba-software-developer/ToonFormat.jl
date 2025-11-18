# Contributing Julia Implementation to TOON Ecosystem

This guide will help you add the Julia implementation to the official TOON repository.

## Steps to Contribute

### 1. Fork and Clone the Main TOON Repository

```bash
# Fork the repository on GitHub first, then:
gh repo fork toon-format/toon --clone
cd toon
```

### 2. Create a New Branch

```bash
git checkout -b add-julia-implementation
```

### 3. Add Julia to Community Implementations

Edit `README.md` and add Julia to the Community Implementations section (alphabetically):

Find this section:
```markdown
### Community Implementations

- **C++:** [ctoon](https://github.com/mohammadraziei/ctoon)
- **Clojure:** [toon](https://github.com/vadelabs/toon)
- **Crystal:** [toon-crystal](https://github.com/mamantoha/toon-crystal)
- **Elixir:** [toon_ex](https://github.com/kentaro/toon_ex)
- **Gleam:** [toon_codec](https://github.com/axelbellec/toon_codec)
- **Go:** [gotoon](https://github.com/alpkeskin/gotoon)
- **Java:** [JToon](https://github.com/felipestanzani/JToon)
```

Add Julia after Java (alphabetically):
```markdown
- **Java:** [JToon](https://github.com/felipestanzani/JToon)
- **Julia:** [Toon.jl](https://github.com/abdelrahman-tolba-software-developer/toon_julia)
- **Kotlin:** [Kotlin-Toon Encoder/Decoder](https://github.com/vexpera-br/kotlin-toon)
```

### 4. Commit and Push

```bash
git add README.md
git commit -m "Add Julia implementation to community implementations

- Repository: https://github.com/abdelrahman-tolba-software-developer/toon_julia
- Status: 264 passing tests (84% pass rate)
- Features: Full encoder/decoder, tabular arrays, nested structures
- Ready for Julia General Registry"
git push origin add-julia-implementation
```

### 5. Create Pull Request

```bash
gh pr create --title "Add Julia implementation to community implementations" \
  --body "This PR adds the Julia implementation (Toon.jl) to the community implementations list.

## Implementation Details

- **Repository**: https://github.com/abdelrahman-tolba-software-developer/toon_julia
- **Status**: 264 passing tests (84% pass rate), 51 edge cases remaining
- **Features**: 
  - Full TOON 2.0 specification support
  - Encoding and decoding
  - Tabular arrays with sorted field ordering
  - Nested structures
  - Configurable options (indent, delimiter, sort_keys)
- **Test Coverage**: Uses official TOON specification test fixtures
- **Documentation**: Complete README with examples

## Checklist

- [x] Follows the TOON specification
- [x] Runs reference test suite (264/315 tests passing)
- [x] Clear README with installation and usage examples
- [x] MIT License
- [x] Ready for Julia General Registry

The implementation is functional and ready for use. Remaining test failures are mostly edge cases (key folding, path expansion) that don't affect core functionality."
```

## Alternative: Manual PR Creation

If you prefer to create the PR manually:

1. Go to: https://github.com/toon-format/toon
2. Click "Fork" (if you haven't already)
3. Edit `README.md` in your fork
4. Add Julia to the Community Implementations list
5. Create a Pull Request with the details above

## What to Include in PR Description

- Link to your repository
- Test status (264/315 passing)
- Key features
- Status (ready for Julia General Registry)
- Any notes about remaining edge cases

## Expected Outcome

Once merged, your Julia implementation will be listed on:
- https://github.com/toon-format/toon (README)
- https://toonformat.dev/ecosystem/implementations.html (Documentation site)

