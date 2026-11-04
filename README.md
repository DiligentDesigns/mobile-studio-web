# mobile-studio-web

**[READ PROJECT_STATE.md FIRST](PROJECT_STATE.md)** when resuming this project from a new conversation, device or contributor. Company-wide governance and source registry are in the private [Software Company Foundation](https://github.com/DiligentDesigns/Software-company-foundation).

This repository hosts the interactive, touchscreen-oriented Mobile Studio web DAW prototype (the existing `index.html` identifies itself as v0.5.0-alpha). Its native C++/Core Audio Mac counterpart is developed separately in [mobile-studio-daw](https://github.com/DiligentDesigns/mobile-studio-daw). A browser prototype is not evidence of native hardware, latency compensation, completed phone compatibility or native/web feature parity.

Before changes, record the exact source SHA, feature/behavior and current tests. Preserve the previous prototype and avoid silently applying experimental native engine assumptions to this browser implementation. The merged [PROJECT_STATE.md](PROJECT_STATE.md) (documentation [PR #1](https://github.com/DiligentDesigns/mobile-studio-web/pull/1)) is an explicit, dated snapshot and next-step gate, not a certified stable release. The source and acceptance state must be reverified against live GitHub and actual browser tests.
