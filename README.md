# Rshell - A Cross-Platform Multi-Protocol C2 Framework

English | **[简体中文](./README_zh-CN.md)**

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](./LICENSE)
![Language](https://img.shields.io/badge/Language-Go-blue)
![GitHub Stars](https://img.shields.io/github/stars/Rubby2001/Rshell---A-Cross-Platform-C2?style=social)
![GitHub Release](https://img.shields.io/github/v/release/Rubby2001/Rshell---A-Cross-Platform-C2)

Rshell is an open-source, multi-platform C2 framework written in Golang, designed for penetration testers and red/blue team engagements.

## Core Features

- **Cross-Platform**: Clients for Windows, Linux and macOS.
- **Multi-Protocol**: Listeners over WebSocket, TCP, KCP, HTTP and cloud object storage (OSS).
- **Evasion & Stealth**: Optional anti-sandbox execution password; in-memory execution (Execute Assembly, Inline Bin, Shellcode Injection, BOF).
- **Interactive Management**: Interactive terminal, file manager, process listing with AV identification, command execution.
- **Modular Plugins**: Rich plugin management with dynamic loading and execution.
- **Decoupled Data**: Custom or random per-client traffic keys, raising the bar for traffic analysis and reverse engineering.

## Getting Started

Download the Rshell binary for your platform and run it.

Specify the port with `-p` (default `8089`):

```bash
./Rshell -p 8089
```

![image-20260429142230230](./assets/image-20260429142230230.png)

## Documentation

For a detailed walkthrough (with screenshots), see the usage documentation:

👉 **[Rshell Usage Documentation (Chinese)](./docs/USAGE.md)**

Topics covered:

- Changing credentials and customizing themes
- Adding protocol listeners and generating clients
- WebDelivery setup
- Client management (terminal, files, process management)
- Windows advanced operations (shellcode generation and in-memory execution)
- Plugin usage and management

> Note: the operator UI currently ships in Chinese; localization is in progress.

## ToDoList

Improvement ideas are updated from time to time. Suggestions and PRs are welcome — feel free to open an issue to discuss.

<details>
<summary>📌 View ToDoList</summary>

- [ ] Interruptible file downloads  [#21](https://github.com/Rubby2001/Rshell---A-Cross-Platform-C2/issues/21)
- [ ] Image hosting for notes
- [ ] WYSIWYG Markdown notes
- [ ] One-click information gathering with results saved into notes

</details>

## Related Projects

- Golang client: https://github.com/Rubby2001/Rshell-client
- Rust client: https://github.com/Rubby2001/Rshell-client-rust
- Web frontend: https://github.com/Rubby2001/Rshell-web

## Disclaimer

1. This project is designed and developed solely for security research, legally authorized testing, and educational purposes, to help security professionals improve defenses and assess system security.
2. **It is strictly forbidden to use this project for any illegal purpose**, including but not limited to:
   - Unauthorized intrusion into systems
   - Cyberattack activities
   - Any violation of applicable laws and regulations
3. Users must ensure they operate under **fully legal authorization**. The developers are not responsible for any abuse.
4. This tool may impact target systems. Users bear all risks and must ensure:
   - Explicit authorization for the target system has been obtained
   - Compliance with local laws and regulations
   - No harm to critical information infrastructure
5. The developers make no promise of stealth, stability or fitness for any particular purpose, and assume no direct or indirect liability arising from the use of this tool.
6. Downloading or using this project means you have read and agree to all terms of this disclaimer.

## License

This project is open-sourced under the [MIT License](./LICENSE).
