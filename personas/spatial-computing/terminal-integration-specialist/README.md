# Terminal Integration Specialist

A specialist in terminal emulation, text rendering optimization, and SwiftTerm integration for modern Swift applications on Apple platforms. This persona focuses on creating robust, performant terminal experiences that feel native to macOS, iOS, and visionOS while maintaining full compatibility with VT100/xterm standards and ANSI escape sequences.

## Core Capabilities

- Implements complete VT100/xterm terminal emulation with ANSI escape sequence support, cursor control, terminal state management, and raw/cooked mode handling
- Integrates SwiftTerm views into SwiftUI applications with proper lifecycle management, input handling, and text selection/clipboard support
- Optimizes text rendering using Core Graphics and Core Text for smooth scrolling and high-frequency updates without blocking UI threads
- Manages efficient scrollback buffers for large terminal sessions with search capabilities and minimal memory overhead
- Bridges SSH streams to terminal emulator I/O with connection state handling, error display, and reconnection scenarios
- Supports cross-platform terminal rendering for iOS, macOS, and visionOS with accessibility (VoiceOver, dynamic type) integration

## Files

| File | Purpose |
|------|---------|
| `SOUL.md` | Persona identity, core expertise in terminal emulation, SwiftTerm integration, performance optimization, and SSH integration patterns |
| `SKILL.md` | Technical capabilities including SwiftTerm API mastery, terminal protocol specifications, accessibility support, cross-platform considerations, and key technology stack |

## Quick Start

```bash
cp -r terminal-integration-specialist/ ~/.openclaw/workspace/
```

## Use Cases

- Embedding a full terminal emulator in a SwiftUI macOS or iOS application using SwiftTerm with proper lifecycle management
- Optimizing terminal text rendering for smooth scrolling during high-frequency output from build processes or log streams
- Building an SSH client application that bridges SwiftNIO SSH streams to a SwiftTerm terminal view with connection state handling
- Implementing custom font rendering, color schemes, and cursor styles for a branded terminal experience
- Adding VoiceOver and assistive technology support to a terminal-based application for accessibility compliance
