<!--
  ╔══════════════════════════════════════════════════════════════════════════════╗
  ║                         AWESOME BEVY — 2026 EDITION                          ║
  ║           A Curated List of Plugins, Tools, Games \& Resources                ║
  ║                    for the Bevy Game Engine (Rust)                           ║
  ╚══════════════════════════════════════════════════════════════════════════════╝

<div align="center">

# 🎮 Awesome Bevy

> A \*\*curated\*\*, \*\*star-ranked\*\*, and \*\*version-tracked\*\* list of everything in the Bevy ecosystem.

[![Bevy](https://img.shields.io/badge/Bevy-0.19-ff69b4?logo=rust&style=for-the-badge)](https://bevy.org/)
[![Rust](https://img.shields.io/badge/Rust-1.85+-orange?logo=rust&style=for-the-badge)](https://www.rust-lang.org/)
[![License](https://img.shields.io/badge/License-CC0-9cf?style=for-the-badge)](https://creativecommons.org/publicdomain/zero/1.0/)
[![Discord](https://img.shields.io/badge/Discord-Join-7289DA?logo=discord&style=for-the-badge)](https://discord.gg/bevy)

**Last Updated:** August 2026 | **Total Entries:** 200+

> 💡 \*\*Note:\*\* The project site moved from `bevyengine.org` to `bevy.org` — update any old bookmarks.

</div>

\---

## 📑 Table of Contents

* [🚀 Quick Start](#-quick-start)
* [📊 Version Matrix](#-version-matrix)
* [🎓 Learning \& Tutorials](#-learning--tutorials)
* [🔧 Dev Tools \& Editors](#-dev-tools--editors)
* [🎨 Graphics \& Rendering](#-graphics--rendering)
* [🖱️ Input](#️-input)
* [⚛️ Physics](#️-physics)
* [🌐 Networking](#-networking)
* [🖥️ UI](#️-ui)
* [🧠 AI](#-ai)
* [🗺️ Tilemaps \& Level Design](#️-tilemaps--level-design)
* [🔊 Audio](#-audio)
* [🎬 Animation \& Tweening](#-animation--tweening)
* [📦 Assets \& Data](#-assets--data)
* [✨ Particles \& Effects](#-particles--effects)
* [🔬 Math \& Simulation](#-math--simulation)
* [🛠️ Development \& Tooling](#️-development--tooling)
* [🎮 Games](#-games)
* [🦀 Useful Rust Tools](#-useful-rust-tools)
* [📚 Uncategorized](#-uncategorized)
* [🔥 Ecosystem Changelog](#-ecosystem-changelog)

\---

## 🚀 Quick Start

```toml
\[dependencies]
bevy = "0.19"
```

```rust
use bevy::prelude::\*;

fn main() {
    App::new()
        .add\_plugins(DefaultPlugins)
        .run();
}
```

> 💡 \*\*Tip:\*\* Use `bevy = { version = "0.19", features = \["dynamic\_linking"] }` for faster compile times during development.

\---

## 📊 Version Matrix

|Bevy Version|Release Date|Notable Highlights|
|:-:|:-:|-|
|**0.19**|Jun 2026|BSN Scenes, Text Input, Contact Shadows, App Settings, Transform Gizmo, Render Graph → Systems|
|0.18|Jan 2026|Fullscreen Materials, Cargo Feature Collections, Font Variations, First-Party Cameras|
|0.17|Sep 2025|Tilemap Chunk Rendering, ViewportNode, Directional UI Nav, Bevy Feathers widgets|
|0.16|Apr 2025|Entity Relationships, `no\_std` support, Required Components, `bevy\_picking`|
|0.15|Nov 2024|Animation Graphs, PCSS Shadows, Gizmos 2.0, `no\_std` prep|
|0.14|Jul 2024|Curves, Required Components preview, Animation Events|

\---

## 🎓 Learning \& Tutorials

|Resource|Description|Stars|
|-|-|:-:|
|[Official Examples](https://github.com/bevyengine/bevy/tree/main/examples)|Always up to date with latest API. The definitive reference.|⭐ 47.8k|
|[Rust API Docs](https://docs.rs/bevy/latest/bevy/)|Inline examples and great descriptions.|—|
|[Official Quick Start Guide](https://bevy.org/learn/quick-start/getting-started/)|The engine's own getting-started walkthrough. Good first stop before anything else.|—|
|[Unofficial Bevy Cheat Book](https://bevy-cheatbook.github.io/)|The go-to book for Bevy concepts — like the Rust Book for Bevy. **Note:** the author has stepped back from maintaining it, so it's frozen in place — great for concepts, but double-check anything version-specific against the official docs.|—|
|[This Week in Bevy](https://thisweekinbevy.com/)|Weekly roundup of engine PRs, new/updated ecosystem crates, and community showcases. Also posted as a YouTube playlist. Honestly the best way to keep a list like this from going stale.|—|
|[Tainted Coders](https://taintedcoders.com/)|Actively updated modern write-ups on Bevy's systems. Also maintains a much bigger, more exhaustive [awesome-bevy list](https://github.com/nolantait/awesome-bevy) worth cross-referencing whenever this list comes up short.|—|
|[Blog Posts](https://bevy.org/news/)|Release notes with code samples for every new API.|—|
|[Community](https://bevy.org/community/)|Discord \& GitHub Discussions — extremely active.|—|
|[Bevy Assets](https://bevy.org/assets/)|The original awesome list. Always check the version as some entries are quite old and the API has changed a lot since then.|—|
|[BevyDex](https://bevydex.dev/dex) / [Bevy Constellation](https://crates.rugaex.com/)|Two community dashboards for browsing which ecosystem crates are updated and popular for a given Bevy version — genuinely useful for exactly the kind of upkeep this list needs.|—|

### Tutorials (Legacy but Valuable)

|Tutorial|Description|Bevy Version|
|-|-|:-:|
|[Snake Tutorial](https://web.archive.org/web/20230301215439/mbuffett.com/posts/bevy-snake-tutorial/)|Classic starter tutorial.|Old|
|[Minesweeper](https://dev.to/qongzi/bevy-minesweeper-introduction-4l7f)|ECS structure for classic games.|Old|
|[Best Practices](https://github.com/tbillington/bevy_best_practices)|Opinionated best practices guide.|Current|
|[Dependency Injection Engine](https://promethia-27.github.io/dependency_injection_like_bevy_from_scratch/introductions.html)|Build an ECS engine from scratch, inspired by Bevy.|Conceptual|
|[Roguelike Tutorial — In Rust](https://bfnightly.bracketproductions.com/)|Not Bevy-specific, but great crossover for ECS architecture.|—|

\---

## 🔧 Dev Tools \& Editors

> ⭐ = GitHub Stars | 🏷️ = Bevy Version | 🏛️ = First-Party (built into Bevy)

|Crate / Tool|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy-inspector-egui](https://github.com/jakobhellermann/bevy-inspector-egui)|Runtime component/entity inspector via egui. v2 uses `Reflect` instead of a custom `Inspectable` trait.|⭐ 1.6k|0.19|
|[bevy\_editor\_pls](https://github.com/jakobhellermann/bevy_editor_pls)|In-game GUI editor with hierarchy and viewport.|⭐ 600+|0.19|
|[bevy\_mod\_debugdump](https://github.com/jakobhellermann/bevy_mod_debugdump)|System execution graph visualizer for schedules.|⭐ 400+|0.19|
|[bevy\_egui](https://github.com/vladbat00/bevy_egui)|Egui integration for Bevy — immediate mode UI. The default pick for debug panels and quick editor-style tooling.|⭐ 1.4k|0.19|
|[blenvy](https://github.com/kaosat-dev/blenvy)|Blender addon + Bevy code for editing Bevy components directly in Blender.|⭐ 400+|0.18|
|[bevy\_mod\_scripting](https://github.com/makspll/bevy_mod_scripting)|Scripting support for Bevy (Lua, Rhai, etc.).|⭐ 300+|0.18|
|[jackdaw](https://github.com/zkat/jackdaw)|Bevy scene editor with hierarchy, inspector, and 3D viewport.|⭐ 200+|0.18|
|[HillVacuum](https://github.com/4Source/HillVacuum)|Bevy-based 2D map editor.|⭐ 200+|0.18|
|[bevy-yoleck](https://github.com/idanarye/bevy-yoleck)|"Your Own Level Editor Creation Kit" — for building a level editor into your own game instead of using a standalone one.|⭐ 150+|0.18|
|[bevy\_trenchbroom](https://github.com/Noxmore/bevy_trenchbroom)|TrenchBroom (the Quake map editor) integration, with `.map`/`.bsp` loading. Great if you want old-school FPS-style level geometry.|⭐ 200+|0.18|
|[bevy\_lint](https://github.com/TheBevyFlock/bevy_cli)|Official-adjacent linter with Bevy-specific lints (auto-fixable, CI-ready).|⭐ 300+|0.19|
|[Bevy CLI](https://github.com/TheBevyFlock/bevy_cli)|Community CLI for scaffolding projects and running web builds. From the same working group behind the Bevy linter.|⭐ 300+|0.19|
|[bevy\_remote\_devtools](https://github.com/reneeichhorn/bevy-remote-devtools)|Remote devtools via the Bevy Remote Protocol.|⭐ 150+|0.19|
|[Bevy Inspection (VSCode)](https://marketplace.visualstudio.com/items?itemName=foxication.bevy-inspection)|VSCode extension for inspecting Bevy apps at runtime.|—|0.19|
|[vscode-bevy-inspector](https://github.com/foxication/vscode-bevy-inspector)|Another VSCode Bevy inspector extension.|⭐ 100+|0.19|
|[Bevy Editor (prototypes)](https://github.com/bevyengine/bevy_editor_prototypes)|The official editor. Still an alpha-quality prototype, but under heavy, funded development. `bevy\_core\_widgets` and the "Bevy Feathers" widget set that will skin it have already landed experimentally — see the [Fifth Birthday post](https://bevy.org/news/bevys-fifth-birthday/) for the full writeup.|—|0.19|
|**🏛️ `bevy\_dev\_tools`**|Built-in: `EasyScreenshotPlugin`, `EasyScreenRecordPlugin`, `DiagnosticsOverlayPlugin`, `TransformGizmoPlugin`, `InfiniteGridPlugin`.|—|0.18+|
|**🏛️ `bevy\_remote`**|Bevy Remote Protocol for external tool integration.|—|0.19|

\---

## 🎨 Graphics \& Rendering

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_hanabi](https://github.com/djeedai/bevy_hanabi)|🎆 GPU particle system — millions of particles, trails, collisions, force fields, 2D/3D. Actively maintained, and about as close as the ecosystem gets to a "standard" particle plugin.|⭐ 1.4k|0.19|
|[bevy\_egui](https://github.com/vladbat00/bevy_egui)|Egui integration — widely used for tools and editors.|⭐ 1.4k|0.19|
|[Vello](https://github.com/linebender/bevy_vello)|Vector rendering with SVG and Lottie support. Now hosted directly under Linebender, the team behind Vello itself.|⭐ 300+|0.18|
|[bevy\_vector\_shapes](https://github.com/james-j-obrien/bevy_vector_shapes)|Immediate-mode rendering of vector shapes.|⭐ 400+|0.19|
|[bevy\_prototype\_lyon](https://github.com/Nilirad/bevy_prototype_lyon)|2D vector shape and path drawing, built on Lyon.|⭐ 350+|0.19|
|[bevy\_sprite3d](https://github.com/FraserLee/bevy_sprite3d)|Use 2D sprites in 3D scenes.|⭐ 200+|0.19|
|[bevy\_feronia](https://github.com/FraserLee/bevy_feronia)|Environment scattering tools \& shaders.|⭐ 150+|0.18|
|[bevy\_firework](https://github.com/djeedai/bevy_firework)|CPU-driven, batch-rendered particle system.|⭐ 200+|0.19|
|[bevy\_enoki](https://github.com/jnhyatt/bevy_enoki)|2D particle system with custom materials. WASM/WebGL2 friendly.|⭐ 150+|0.19|
|[bevy\_spritesheet\_animation](https://github.com/jnhyatt/bevy_spritesheet_animation)|Easy 2D/3D sprite animation from spritesheets.|⭐ 200+|0.19|
|[noisy\_bevy](https://github.com/jnhyatt/noisy_bevy)|Simple noise primitives for WGSL and Rust.|⭐ 150+|0.19|
|[bevy\_2d\_screen\_space\_lightmaps](https://github.com/goto64/bevy_2d_screen_space_lightmaps)|Simple 2D lighting via screen-space lightmaps.|⭐ 100+|0.18|
|[bevy\_light\_2d](https://github.com/jgayfer/bevy_light_2d)|General-purpose drop-in 2D lighting plugin.|⭐ 100+|0.18|
|[bevy-magic-light-2d](https://github.com/zaycev/bevy-magic-light-2d)|Experimental dynamic 2D global illumination via SDF ray-marching and bounced light.|⭐ 200+|0.18|
|[shadplay](https://github.com/alphastrata/shadplay)|Real-time WGSL shader visualization tool.|⭐ 150+|0.18|
|[bevy\_mod\_outline](https://github.com/komadori/bevy_mod_outline)|Mesh outlines via vertex extrusion \& jump flood.|⭐ 200+|0.18|
|[bevy\_mod\_mipmap\_generator](https://github.com/DGriffin91/bevy_mod_mipmap_generator)|Basic mipmap generator for Bevy textures.|⭐ 100+|0.18|
|[bevy\_water](https://github.com/Neopallium/bevy_water)|Dynamic ocean material for Bevy.|⭐ 150+|0.18|
|[bevy\_march](https://github.com/NiseVoid/bevy_march)|Ray marcher alongside regular mesh rendering.|⭐ 100+|0.18|
|[bevy\_materialize](https://github.com/Noxmore/bevy_materialize)|Load, store, and apply type-erased materials.|⭐ 100+|0.18|
|**🏛️ `FullscreenMaterial`**|High-level fullscreen post-processing without custom render features.|—|0.18|
|**🏛️ `ContactShadows`**|Better shadow detail for close-proximity objects.|—|0.19|
|**🏛️ `RectangularAreaLight`**|Area lighting support.|—|0.19|
|**🏛️ `Solari`**|Experimental real-time path-traced renderer, improved each release.|—|0.19|

\---

## 🖱️ Input

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[leafwing-input-manager](https://github.com/Leafwing-Studios/leafwing-input-manager)|Action-based input for keyboard, mouse, gamepad. Parts of its design are on track to be upstreamed into Bevy itself eventually.|⭐ 900+|0.19|
|[bevy\_enhanced\_input](https://github.com/simgine/bevy_enhanced_input)|Observer/component-based input manager modeled on Unreal's Enhanced Input. It's become the up-and-coming alternative to the Leafwing manager, and its author has floated eventually upstreaming it as Bevy's own input abstraction.|⭐ 400+|0.19|
|[bevy-mouse-tracking](https://github.com/JoJoJet/bevy-mouse-tracking)|Small utility for getting the cursor's world-space position, which Bevy doesn't expose directly out of the box.|⭐ 150+|0.18|
|[bevy\_pancam](https://github.com/johanhelsing/bevy_pancam)|Drag-to-pan and scroll-to-zoom for orthographic cameras — handy for 2D and city-builder-style games.|⭐ 400+|0.19|
|[bevy\_flycam](https://github.com/sburris0/bevy_flycam)|Basic first-person fly camera.|⭐ 300+|0.19|
|[bevy\_third\_person\_camera](https://github.com/The-DevBlog/bevy_third_person_camera)|Third-person camera with orbit, follow, collision.|⭐ 200+|0.18|
|[bevy\_editor\_cam](https://github.com/aevyrie/bevy_editor_cam)|Camera controller for editors and CAD applications.|⭐ 150+|0.18|
|[bevy\_ahoy](https://github.com/janhohenheim/bevy_ahoy)|Lighter kinematic 3D character controller, built specifically for Avian.|⭐ 100+|0.18|
|[bevy-tnua](https://github.com/idanarye/bevy-tnua)|A "floating" character controller that sits on top of Rapier or Avian.|⭐ 200+|0.18|
|**🏛️ `AutomaticDirectionalNavigation`**|Built-in gamepad/keyboard UI navigation.|—|0.18|

> 💡 Click/hover/drag picking now ships in Bevy core as `bevy::picking`, so `bevy\_mod\_picking` is mostly relevant to older versions at this point.

\---

## ⚛️ Physics

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[Avian](https://github.com/avianphysics/avian)|ECS-native 2D and 3D physics. **Successor to Bevy XPBD.** No separate physics world to keep in sync, and close to feature parity with Rapier at this point. Collision hooks, observable events, physics diagnostics, interpolation, and `no\_std` support.|⭐ 3.1k|0.19|
|[bevy\_rapier](https://github.com/dimforge/bevy_rapier)|Official Rapier 2D/3D physics integration. More battle-tested than Avian if you want the safer, more proven pick.|⭐ 1.6k|0.19|
|[Bevy raycast](https://github.com/aevyrie/bevy_mod_raycast)|Simple raycast system for meshes. Basic mesh raycasting is also available via core `bevy::picking` now.|⭐ 400+|0.18|
|[bevy-tnua](https://github.com/idanarye/bevy-tnua)|A "floating" character controller that sits on top of Rapier or Avian.|⭐ 200+|0.18|
|[bevy\_ahoy](https://github.com/janhohenheim/bevy_ahoy)|Lighter kinematic 3D character controller, built specifically for Avian.|⭐ 100+|0.18|
|[bevy\_heavy](https://github.com/avianphysics/bevy_heavy)|Mass properties for Bevy's geometric primitives.|⭐ 100+|0.19|
|[bevy\_transform\_interpolation](https://github.com/Jondolf/bevy_transform_interpolation)|Transform interpolation for fixed timesteps.|⭐ 100+|0.19|
|[avian\_pickup](https://github.com/janhohenheim/avian_pickup)|Pick up dynamic rigid bodies in Avian.|⭐ 100+|0.19|
|[bevy\_mod\_inverse\_kinematics](https://github.com/Kurble/bevy_mod_inverse_kinematics)|Inverse kinematics plugin for Bevy.|⭐ 100+|0.18|
|**🏛️ `bevy\_picking`**|First-party pointer events: hover, click, drag, input-agnostic. Built-in since Bevy 0.16.|—|0.16+|

> ⚠️ `bevy\_xpbd` has been \*\*rebranded as Avian\*\* and moved to [AvianPhysics/avian](https://github.com/avianphysics/avian).

\---

## 🌐 Networking

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[Lightyear](https://github.com/cBournhonesque/lightyear)|Full-featured server-authoritative networking with client-side prediction, interpolation, and rollback built in. Supports WASM via WebTransport/WebSockets, and now builds on top of bevy\_replicon under the hood.|⭐ 1.1k|0.19|
|[bevy\_replicon](https://github.com/simgine/bevy_replicon)|A leaner, transport-agnostic world-replication crate — bring your own I/O (Renet, Lightyear, QUIC, etc). Increasingly the base layer other networking crates build on.|⭐ 700+|0.19|
|[Renet](https://github.com/lucaspoffo/renet)|Server/Client network library for multiplayer games. Fast-paced games.|⭐ 800+|0.19|
|[bevy\_renet](https://github.com/lucaspoffo/renet)|Bevy plugin for Renet.|⭐ 600+|0.19|
|[renet2](https://github.com/UkoeHB/renet2)|A community fork of Renet aimed at fast-paced competitive games, adding things the original lacks, like WASM/browser transport.|⭐ 300+|0.19|
|[Matchbox](https://github.com/johanhelsing/matchbox)|P2P WebRTC networking for Rust (WASM + native). Pairs with GGRS.|⭐ 1.0k|0.19|
|[bevy\_matchbox](https://github.com/johanhelsing/matchbox)|Bevy integration for Matchbox sockets.|⭐ 1.0k|0.19|
|[bevy\_ggrs](https://github.com/gschup/bevy_ggrs)|P2P rollback networking plugin. Uses Matchbox for browser P2P.|⭐ 500+|0.19|
|[bevy\_quinnet](https://github.com/Henauxg/bevy_quinnet)|Client/server networking over QUIC.|⭐ 400+|0.19|
|[aeronet](https://github.com/aecsocket/aeronet)|Bevy-native networking primitives: fragmentation, reliability, ordering.|⭐ 300+|0.19|
|[bevy\_rewind](https://github.com/NiseVoid/bevy_rewind)|Server-authoritative rollback inspired by Rocket League.|⭐ 150+|0.18|
|[bevy\_streaming](https://github.com/rlamarche/bevy_streaming)|Cloud gaming via WebRTC streaming.|⭐ 100+|0.18|
|[bevy\_oxr](https://github.com/awtterpip/bevy_oxr)|OpenXR (and future WebXR) support for Bevy.|⭐ 200+|0.18|
|[bevygap](https://github.com/RJ/bevygap)|Autoscaling multiplayer servers (Edgegap + Lightyear).|⭐ 100+|0.19|
|[bevy\_replicon\_renet](https://github.com/simgine/bevy_replicon_renet)|Renet backend for bevy\_replicon.|⭐ 200+|0.19|
|[bevy\_replicon\_quinnet](https://github.com/Henauxg/bevy_replicon_quinnet)|Quinnet backend for bevy\_replicon.|⭐ 150+|0.19|
|[aeronet\_replicon](https://github.com/aecsocket/aeronet)|Aeronet backend for bevy\_replicon.|⭐ 300+|0.19|
|[bevy\_replicon\_repair](https://github.com/UkoeHB/bevy_replicon_repair)|Client state repair across reconnects.|⭐ 100+|0.19|

> 📖 \*\*Tutorial:\*\* [Extreme Bevy — P2P Web Game with GGRS + Matchbox](https://johanhelsing.studio/posts/extreme-bevy)

\---

## 🖥️ UI

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_egui](https://github.com/vladbat00/bevy_egui)|Immediate-mode GUI via egui. The default pick for debug panels and quick editor-style tooling.|⭐ 1.4k|0.19|
|[Lunex](https://github.com/bytestring-net/bevy-lunex)|Path-based retained layout engine with an impressive demo. Maintained largely by one university student, so don't expect fast updates during the semester.|⭐ 400+|0.19|
|[sickle\_ui](https://github.com/UmbraLuminosa/sickle_ui)|A widget library built on top of `bevy\_ui`, still commonly reached for when building complex in-game menus. Check recent commits before depending on it directly — upstream activity has slowed lately.|⭐ 300+|0.18|
|[haalka](https://github.com/databasedav/haalka)|An ergonomic reactive UI library built on FRP-style signals — a different approach from Lunex or sickle\_ui.|⭐ 150+|0.18|
|[bevy\_hui](https://github.com/Lommix/bevy_hui)|Component-based UI using XML/HTML with hot reload.|⭐ 100+|0.18|
|[bevy\_flair](https://github.com/eckz/bevy_flair)|Bevy UI styling using CSS-like syntax.|⭐ 100+|0.18|
|[bevy\_immediate](https://github.com/PPakalns/bevy_immediate)|Immediate mode UI library, simple and extensible.|⭐ 100+|0.18|
|[bevy\_material\_ui](https://github.com/edgarhsanchez/bevy_material_ui)|Material UI design system for Bevy.|⭐ 100+|0.18|
|[bevy\_ui\_anchor](https://github.com/TotalKrill/bevy_ui_anchor)|Microlibrary for UI anchoring.|⭐ 100+|0.18|
|[bevy\_healthbar\_3d](https://github.com/sparten11740/bevy_health_bar3d)|Billboard health bars as shaders.|⭐ 150+|0.18|
|[transform-gizmo](https://github.com/urholaukkarinen/transform-gizmo)|3D transformation gizmo widget.|⭐ 200+|0.18|
|[bevy\_ui\_text\_input](https://github.com/ickshonpe/bevy_ui_text_input)|Text input using cosmic text.|⭐ 100+|0.18|
|[bevy\_simple\_text\_input](https://github.com/rparrett/bevy_simple_text_input)|Simple single-line text input widget.|⭐ 100+|0.18|
|[bevy\_pretty\_text](https://github.com/void-scape/pretty-text)|Text2D effects library.|⭐ 100+|0.18|
|[bevy\_rich\_text3d](https://github.com/mintlu8/bevy_rich_text3d)|Mesh-based 3D text implementation.|⭐ 100+|0.18|
|**🏛️ `bevy\_ui` + `bevy\_feathers`**|Bevy's own emerging first-party styled widget set (buttons, checkboxes, sliders, scrollbars…), shipped experimentally starting in 0.17 to eventually power both the official Editor and regular app UI. The closest thing to an "official" answer here.|—|0.17+|
|**🏛️ `ViewportNode`**|Render camera output directly inside a UI node.|—|0.17+|
|**🏛️ `EditableText`**|Built-in text entry with cursor, selection, clipboard, IME, multiline, and bidirectional text support.|—|0.19+|
|**🏛️ `Popover`**|Automatic popup positioning (inspired by floating-ui).|—|0.18+|
|**🏛️ `MenuPopup`**|Dropdown menu with keyboard navigation.|—|0.18+|

\---

## 🧠 AI

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[big-brain](https://github.com/zkat/big-brain)|A Utility AI library (scorers + actions + "thinkers"). Probably the most widely used general-purpose game-AI crate in the ecosystem today.|⭐ 1.3k|0.19|
|[Bonsai](https://github.com/Sollimann/bonsai)|Behaviour trees for AI agents.|⭐ 400+|0.18|
|[seldom\_state](https://github.com/Seldom-SE/seldom_state)|Component-based finite state machine — good for player/enemy state and driving animation. Pairs well alongside big-brain rather than competing with it.|⭐ 200+|0.18|
|[bevy\_behave](https://github.com/RJ/bevy_behave)|Behaviour trees with on-demand entity spawning for task nodes.|⭐ 150+|0.18|
|[bevy\_gauge](https://github.com/DEMIURGE-studio/bevy_gauge)|Flexible stat and modifier system (RPG stats).|⭐ 100+|0.18|
|[vleue\_navigator](https://github.com/vleue/vleue_navigator)|Navmesh pathfinding for Bevy.|⭐ 200+|0.19|
|[bevy\_northstar](https://github.com/JtotheThree/bevy_northstar)|Hierarchical pathfinding, a good fit for grid/tile-based games.|⭐ 100+|0.18|

\---

## 🗺️ Tilemaps \& Level Design

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_ecs\_tilemap](https://github.com/StarArawn/bevy_ecs_tilemap)|The standard ECS-friendly tile-rendering base layer for 2D games — still actively maintained. One tile = one entity, chunked rendering, isometric/hex, GPU animations.|⭐ 1.3k|0.19|
|[bevy\_ecs\_ldtk](https://github.com/Trouv/bevy_ecs_ldtk)|Editor-format integration for LDtk maps, built on top of `bevy\_ecs\_tilemap`.|⭐ 400+|0.19|
|[bevy\_ecs\_tiled](https://github.com/adrien-bon/bevy_ecs_tiled)|Editor-format integration for Tiled maps, built on top of `bevy\_ecs\_tilemap`.|⭐ 300+|0.19|
|[bevy\_simple\_tilemap](https://github.com/forbjok/bevy_simple_tilemap)|Refreshingly simple tilemap when you just need a grid of rectangular tiles.|⭐ 150+|0.19|
|[bevy\_procedural\_tilemaps](https://github.com/jamesfebin/bevy_procedural_tilemaps)|Wave Function Collapse / Model Synthesis tile generation.|⭐ 100+|0.18|
|[bevy\_rpack](https://github.com/Leinnan/rpack)|Create tilemaps in seconds from packed sprites.|⭐ 100+|0.18|
|[bevy\_trenchbroom](https://github.com/Noxmore/bevy_trenchbroom)|TrenchBroom (the Quake map editor) integration, `.map`/`.bsp` loading. Great if you want old-school FPS-style level geometry.|⭐ 200+|0.18|
|[bevy-yoleck](https://github.com/idanarye/bevy-yoleck)|"Your Own Level Editor Creation Kit" — for building a level editor into your own game.|⭐ 150+|0.18|
|[skein](https://github.com/rust-adventure/skein)|Convert glTF extras to Bevy Components via reflection.|⭐ 100+|0.18|
|**🏛️ `TilemapChunk`**|First-party fast chunk-based tilemap rendering.|—|0.17+|

\---

## 🔊 Audio

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_seedling](https://github.com/CorvusPrudens/bevy_seedling)|Newer integration built on the Firewheel audio engine, with a more modern node-graph style mixer. Effects routing, HRTF spatialization, custom audio processors, and web backend support.|⭐ 200+|0.19|
|[bevy\_kira\_audio](https://github.com/NiklasEi/bevy_kira_audio)|Swaps in the Kira audio engine for real mixing, channels, looping and spatial audio — the de facto standard beyond Bevy's built-in audio.|⭐ 600+|0.19|
|[bevy\_fmod](https://github.com/Salzian/bevy_fmod)|Idiomatic FMOD audio engine integration.|⭐ 200+|0.18|
|[bevy\_oddio](https://github.com/harudagondi/bevy_oddio)|Oddio backend for advanced 3D spatial sound.|⭐ 100+|0.18|
|[bevy\_fundsp](https://github.com/harudagondi/bevy_fundsp)|Fundsp backend for sound synthesis and effects.|⭐ 100+|0.18|

> 🎵 \*\*bevy\_seedling\*\* is the new advanced audio solution displacing `bevy\_kira\_audio` for many projects.

\---

## 🎬 Animation \& Tweening

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_tweening](https://github.com/djeedai/bevy_tweening)|Tween any component/asset field with lenses, sequences, and parallel animations.|⭐ 600+|0.19|
|[bevy\_easings](https://github.com/vleue/bevy_easings)|Similar easing-driven animation helper.|⭐ 300+|0.19|
|[bevy\_tween](https://github.com/Multirious/bevy_tween)|Flexible tweening with procedural and keyframe animation support.|⭐ 200+|0.19|
|[bevy\_animation\_graph](https://github.com/mbrea-c/bevy_animation_graph)|Node-graph-based animation blending, closer to what Unity's or Unreal's animation graphs offer.|⭐ 150+|0.18|
|[bevy\_lookup\_curve](https://github.com/villor/bevy_lookup_curve)|Editable lookup curves for animation.|⭐ 100+|0.18|
|[bevy\_spritesheet\_animation](https://github.com/merwaaan/bevy_spritesheet_animation)|Easy 2D/3D spritesheet animation.|⭐ 200+|0.19|

\---

## 📦 Assets \& Data

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_asset\_loader](https://github.com/NiklasEi/bevy_asset_loader)|Organizes asset loading behind app states, so you're not hand-rolling loading-screen bookkeeping. Declarative loading with `AssetCollection` derive.|⭐ 700+|0.19|
|[bevy\_proto](https://github.com/MrGVSV/bevy_proto)|Load entity definitions from files with inheritance and hierarchies, similar to Unity prefabs.|⭐ 400+|0.19|
|[bevy\_common\_assets](https://github.com/NiklasEi/bevy_common_assets)|Drop-in loaders for common data formats (RON, JSON, YAML, etc), handy for data-driven game content.|⭐ 200+|0.19|
|[bevy\_embedded\_assets](https://github.com/vleue/bevy_embedded_assets)|Embed assets directly into your binary.|⭐ 150+|0.19|
|[bevy-persistent](https://github.com/umut-sahin/bevy-persistent)|Easily manage resources that persist across sessions.|⭐ 200+|0.18|
|[bevy\_simple\_prefs](https://github.com/rparrett/bevy_simple_prefs)|Persist multiple Resources to a single file.|⭐ 100+|0.18|
|[bevy\_assetio\_zip](https://github.com/katharostech/bevy_assetio_zip)|Load assets from obfuscated zip bundles.|⭐ 100+|0.18|
|[bevy\_obj](https://github.com/AmionSky/bevy_obj)|Wavefront OBJ mesh asset loader.|⭐ 150+|0.19|
|[bevy\_svg](https://github.com/Weasy666/bevy_svg)|SVG drawing for Bevy (simple but functional).|⭐ 150+|0.18|
|[moonshine\_save](https://github.com/Zeenobit/moonshine_save)|Save/load framework for Bevy game engine.|⭐ 200+|0.19|
|[leafwing\_manifest](https://github.com/Leafwing-Studios/leafwing_manifest)|Data-driven content generation for Bevy.|⭐ 150+|0.19|
|[bevy\_rand](https://github.com/Bluefinger/bevy_rand)|`rand`, but wired into Bevy's ECS — reflectable, state/scene-friendly RNG resources instead of one bare global generator.|⭐ 200+|0.19|
|[bevy\_shuffle\_bag](https://github.com/janhohenheim/bevy_shuffle_bag)|Shuffle bag for non-repeating random picks.|⭐ 100+|0.19|
|[bevy\_play\_card](https://github.com/Rabbival/bevy_play_card)|Card game utilities for Bevy.|⭐ 100+|0.19|
|[bevy\_http\_client](https://github.com/foxzool/bevy_http_client)|Simple HTTP client for native and WASM.|⭐ 100+|0.19|
|[bevy\_web\_asset](https://github.com/johanhelsing/bevy_web_asset)|Load assets over HTTP in WASM builds.|⭐ 150+|0.18|
|[bevy\_mod\_reqwest](https://github.com/TotalKrill/bevy_mod_reqwest)|Reqwest-based HTTP client for Bevy.|⭐ 100+|0.18|

\---

## ✨ Particles \& Effects

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_hanabi](https://github.com/djeedai/bevy_hanabi)|GPU particle system — millions of particles, trails, collisions, force fields, 2D/3D. The ecosystem's closest thing to a "standard" particle plugin.|⭐ 1.4k|0.19|
|[bevy\_firework](https://github.com/mbrea-c/bevy_firework)|CPU-driven, batch-rendered particles.|⭐ 200+|0.19|
|[bevy\_enoki](https://github.com/Lommix/bevy_enoki)|2D particles with custom materials. WASM/WebGL2 friendly.|⭐ 150+|0.19|

\---

## 🔬 Math \& Simulation

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[Particular](https://github.com/Canleskis/particular)|N-body simulation with great performance.|⭐ 300+|0.18|
|[big\_space](https://github.com/aevyrie/big_space)|Floating origin for spaces larger than the universe.|⭐ 200+|0.19|
|[noiz](https://github.com/ElliottjPierce/noiz)|Configurable, blazingly fast noise library for Bevy.|⭐ 150+|0.19|
|[hexx](https://github.com/ManevilleF/hexx)|Hexagonal tools library for Rust.|⭐ 300+|0.19|

\---

## 🛠️ Development \& Tooling

|Crate / Tool|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_game\_template](https://github.com/niklasei/bevy_game_template)|Full game template: CI/CD for web, Windows, Linux, macOS, iOS, Android.|⭐ 1.1k|0.19|
|[bevy\_github\_ci\_template](https://github.com/bevyengine/bevy_github_ci_template)|GitHub Actions CI/CD template with itch.io publishing.|⭐ 500+|0.19|
|[bevy\_new\_2d](https://github.com/TheBevyFlock/bevy_new_2d)|Official 2D game starter template.|⭐ 300+|0.19|
|[bevy\_quickstart](https://github.com/TheBevyFlock/bevy_quickstart)|Official quickstart template.|⭐ 200+|0.19|
|[bevy\_space](https://github.com/perlindgren/bevy-space)|Space game starter template.|⭐ 150+|0.19|
|[limitpush](https://github.com/heydocode/limitpush)|Another Bevy game template.|⭐ 100+|0.19|
|[bevy\_lint](https://github.com/TheBevyFlock/bevy_cli)|Bevy-specific linter with auto-fixes. CI-ready.|⭐ 300+|0.19|
|[Bevy CLI](https://github.com/TheBevyFlock/bevy_cli)|Scaffolding, web builds, linting.|⭐ 300+|0.19|
|[bevy\_framepace](https://github.com/aevyrie/bevy_framepace)|Framepacing and framelimiting for Bevy.|⭐ 200+|0.19|
|[bevy\_console](https://github.com/RichoDemus/bevy-console)|Half-Life inspired in-game console with clap parsing.|⭐ 200+|0.18|
|[bevy\_mod\_debugdump](https://github.com/jakobhellermann/bevy_mod_debugdump)|Visualize system schedules as graphs.|⭐ 400+|0.19|
|[flamegraph](https://github.com/flamegraph-rs/flamegraph)|Performance profiling with easy-to-read reports.|⭐ 2.9k|Any|
|[Criterion](https://github.com/bheisler/criterion.rs)|Benchmarking library for Rust.|⭐ 3.5k|Any|
|[cargo-make](https://github.com/sagiegurari/cargo-make)|Task runner for build automation.|⭐ 1.5k|Any|
|[hyperfine](https://github.com/sharkdp/hyperfine)|Command-line benchmarking tool.|⭐ 2.9k|Any|
|[VSCode snippets for Bevy](https://github.com/pixldev/bevy-snippets)|Save time on repetitive Bevy code.|⭐ 200+|Any|

\---

## 🎮 Games

### 🏆 Released Games

|Game|Description|Platform|
|-|-|:-:|
|[Tiny Glade](https://store.steampowered.com/app/2198150/Tiny_Glade/)|Relaxing castle doodling. Custom renderer + Bevy ECS. Picked up nominations at the 2024 Steam Awards, the 2024 Independent Games Festival, and the 2025 BAFTA Games Awards (Technical Achievement).|Steam|
|[Tunnet](https://puzzled-squid.itch.io/tunnet)|Underground computer network builder.|Itch.io|
|[LongStory 2](https://store.steampowered.com/app/2427820/LongStory_2/)|Sequel to the award-winning LongStory visual novel/dating sim.|Steam|
|[POLDERS / Waterwolf](https://store.steampowered.com/)|Dutch city builder — fight the sea.|Steam|
|[Exofactory](https://store.steampowered.com/)|Factory builder with belts and automation.|Steam|
|[Greenfeet Haven](https://store.steampowered.com/)|Atmospheric building game.|Steam|

### 🚧 Upcoming Games

|Game|Description|Platform|
|-|-|:-:|
|[Jarl](https://www.jarl-game.com/)|Norse fantasy colony simulator. Still no announced release date — in active playtesting, followed mainly through Discord.|Steam|
|[Times of Progress](https://store.steampowered.com/app/2628450/Times_of_Progress/)|Industrial revolution city builder.|Steam|
|[Settletopia](https://store.steampowered.com/app/3533480/Settletopia/)|Colony sim with multiplayer, recently picked up modding support.|Steam|
|[Unhaunter](https://github.com/deavid/unhaunter)|2D isometric investigation game, still under active development.|GitHub|
|[One Planet](https://buttondown.email/oneplanet/)|Climate crisis grand strategy, now officially announced on Steam.|Newsletter/Steam|
|[To Build a Home](https://thisweekinbevy.com/)|Atmospheric building game (playtests ongoing).|—|
|[Rare Episteme](https://thisweekinbevy.com/)|Narrative/exploration game.|—|
|[Abysm](https://thisweekinbevy.com/)|2024 community spooky jam winner.|Steam|

### 🧪 Open Source Prototypes

|Project|Description|⭐|
|-|-|:-:|
|[Build A Better Buddy](https://github.com/cart/build_a_better_buddy)|Cute auto-battler.|⭐ 400+|
|[Card Combinator](https://github.com/cart/card_combinator)|Card resource management (Stacklands-like).|⭐ 300+|
|[Flock fusion](https://github.com/paul-hansen/bevy-jam-2)|Flocking simulator game.|⭐ 200+|
|[One Clicker](https://github.com/Red-Teapot/CombinerClicker)|Arithmetic clicker/factory game.|⭐ 150+|
|[Fish Folk Punchy](https://github.com/fishfolk/punchy)|2.5D side-scroller beat-em-up.|⭐ 400+|
|[Digital Extinction](https://github.com/DigitalExtinction/Game)|3D RTS game.|⭐ 500+|
|[Doomé](https://github.com/Patryk27/doome)|Doom clone (Game Off 2022). Custom components.|⭐ 300+|
|[Chainboom](https://github.com/Bevy-Jam-6/chainboom)|A Bevy Jam 6 entry — destroy enemy bases while managing the chain reaction of explosions that follows.|⭐ 100+|
|[nannou](https://github.com/nannou-org/nannou)|Creative coding framework (uses Bevy).|⭐ 6.7k|

### 🎲 Bevy Game Jams

Most jam games are open source — great for real-world usage examples.

|Jam|Date|Theme|
|-|:-:|-|
|[Bevy Jam 1](https://itch.io/jam/bevy-jam-1)|2022|—|
|[Bevy Jam 2](https://itch.io/jam/bevy-jam-2)|2022|—|
|[Bevy Jam 3](https://itch.io/jam/bevy-jam-3)|2023|—|
|[Bevy Jam 4](https://itch.io/jam/bevy-jam-4)|2023|—|
|[Bevy Jam 5](https://itch.io/jam/bevy-jam-5)|2024|—|
|[Bevy Jam 6](https://itch.io/jam/bevy-jam-6)|2025|—|
|[Bevy Jam 7](https://itch.io/jam/bevy-jam-7)|Feb 2026|"Extremely Incohesive Fever Dream"|
|[Bevy Spooky Jam](https://itch.io/jam/bevy-spooky-jam)|Off-cycle|Spooky themed|

> 🎮 See [itch.io's "bevy" tag](https://itch.io/games/tag-bevy) for every game tagged Bevy on itch, jam or not — the easiest way to browse broadly and catch whatever's newest.

> 📋 See [Awesome Prod](https://github.com/Vrixyz/bevy_awesome_prod) for a more complete list of production projects using Bevy commercially (analysis/observability tooling, CAD, streaming renderers, and more).

\---

## 🦀 Useful Rust Tools (General)

|Tool|Description|⭐|
|-|-|:-:|
|[arewegameyet](https://arewegameyet.rs/)|General Rust gamedev collection. Not specific to Bevy.|—|
|[rand](https://github.com/rust-random/rand)|Randomness library.|⭐ 1.5k|
|[Serde](https://github.com/serde-rs/serde)|Serialization framework.|⭐ 9k|
|[Rayon](https://github.com/rayon-rs/rayon)|Data parallelism (`par\_iter()`).|⭐ 10k|
|[petgraph](https://github.com/petgraph/petgraph)|General-purpose graph data structures.|⭐ 3k|
|[pathfinding](https://github.com/samueltardieu/pathfinding)|A\*, Dijkstra, and more. A fine building block if `vleue\_navigator` or `bevy\_northstar` don't fit.|⭐ 1k|
|[Criterion](https://github.com/bheisler/criterion.rs)|Benchmarking library.|⭐ 3.5k|
|[flamegraph](https://github.com/flamegraph-rs/flamegraph)|Performance profiling.|⭐ 2.9k|
|[colorgrad](https://github.com/mazznoer/colorgrad-rs)|Color gradient generation.|⭐ 300+|
|[hyperfine](https://github.com/sharkdp/hyperfine)|Command-line benchmarking.|⭐ 2.9k|
|[cargo-make](https://github.com/sagiegurari/cargo-make)|Task runner for build automation.|⭐ 1.5k|

\---

## 📚 Uncategorized

|Crate|Description|⭐|🏷️|
|-|-|:-:|:-:|
|[bevy\_combat](https://github.com/ElliotB256/bevy_combat)|Combat system utilities for Bevy.|⭐ 200+|0.18|
|[bevy-in-web-worker](https://github.com/jinleili/bevy-in-web-worker)|Run Bevy in a Web Worker, interact with HTML.|⭐ 100+|0.19|
|[bevy\_flurx](https://github.com/not-elm/bevy_flurx)|Coroutines in Bevy.|⭐ 150+|0.18|
|[beet](https://github.com/mrchantey/beet)|Bevy application development and publishing systems.|⭐ 100+|0.18|
|[bevy\_auto\_plugin](https://github.com/StrikeForceZero/bevy_auto_plugin)|Auto-registration macros for plugins.|⭐ 100+|0.19|
|[bevy\_ios\_safearea](https://github.com/rustunit/bevy_ios_safearea)|Query iOS device safe area insets.|⭐ 100+|0.18|
|[rmv-bevy-testing-tools](https://github.com/rmvermeulen/rmv-bevy-testing-tools)|Tools to make testing Bevy stuff easier.|⭐ 100+|0.18|

\---

## 🔥 Ecosystem Changelog

> What changed since the last version of this list.

|Old|New / Status|Impact|
|-|-|:-:|
|`bevy\_xpbd`|→ **Avian** ([AvianPhysics/avian](https://github.com/avianphysics/avian))|🔴 High|
|`bevy\_mod\_picking`|→ **First-party `bevy\_picking`** (built-in since 0.16)|🔴 High|
|`bevy\_kira\_audio`|→ **bevy\_seedling** (new advanced audio solution)|🟡 Medium|
|No built-in text input|→ **`EditableText`** (Bevy 0.19)|🔴 High|
|No built-in settings|→ **`SettingsPlugin`** (Bevy 0.19)|🟡 Medium|
|Complex render graph|→ **Render Graph as Systems** (Bevy 0.19)|🟡 Medium|
|No built-in camera controllers|→ **`FreeCamera`**, `bevy\_camera\_controller` (Bevy 0.18)|🟢 Low|
|No built-in UI widgets|→ **`bevy\_feathers`** standard widgets (Bevy 0.17+)|🟡 Medium|
|`bevyengine.org`|→ **`bevy.org`** (site moved)|🟢 Low|
|`bevy 0.14` era|→ **Bevy 0.19** (current as of Aug 2026)|🔴 High|

\---

## 🏅 Star Rankings (Top 20)

|Rank|Crate|⭐|Category|
|:-:|-|:-:|-|
|1|**bevy** (engine)|47.8k|Engine|
|2|**nannou**|6.7k|Creative Coding|
|3|**Avian**|3.1k|Physics|
|4|**bevy-inspector-egui**|1.6k|Dev Tools|
|5|**bevy\_rapier**|1.6k|Physics|
|6|**bevy\_egui**|1.4k|UI / Graphics|
|7|**bevy\_hanabi**|1.4k|Graphics|
|8|**big-brain**|1.3k|AI|
|9|**bevy\_ecs\_tilemap**|1.3k|Tilemaps|
|10|**bevy\_game\_template**|1.1k|Template|
|11|**Lightyear**|1.1k|Networking|
|12|**Matchbox**|1.0k|Networking|
|13|**bevy\_kira\_audio**|600+|Audio|
|14|**bevy\_tweening**|600+|Animation|
|15|**bevy\_ggrs**|500+|Networking|
|16|**Digital Extinction**|500+|Game|
|17|**bevy\_github\_ci\_template**|500+|Dev Tools|
|18|**bevy\_replicon**|700+|Networking|
|19|**bevy\_renet**|600+|Networking|
|20|**bevy\_asset\_loader**|700+|Assets|

\---

<div align="center">

## 🤝 Contributing

> This list is community-curated. PRs welcome!

**Criteria for inclusion:**

* ✅ Actively maintained (or clearly marked unmaintained)
* ✅ Compatible with Bevy 0.16+ (preferred: 0.18+)
* ✅ Open source with clear license
* ✅ Useful to the broader Bevy community

**Maintained by:** The Bevy Community  
**Last updated:** August 2026  
**Bevy version:** 0.19

[![Bevy](https://img.shields.io/badge/Made%20with-Bevy-ff69b4?logo=rust&style=flat-square)](https://bevy.org/)

</div>

