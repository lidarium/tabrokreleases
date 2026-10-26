# Third-Party Notices

Attribution notices for third-party open-source components bundled with or used by Tabrok.
Each component remains subject to its own license. The complete license texts are in the
[`THIRD-PARTY-LICENSES/`](THIRD-PARTY-LICENSES/) directory of this repository and are
redistributed with the application at `Tabrok.app/Contents/Resources/THIRD-PARTY-LICENSES/`.
These notices do not affect the proprietary license of Tabrok's own code (see `LICENSE`).

## 1. Application Framework & Runtime

- **Electron** — MIT License — Copyright (c) GitHub Inc. Full text ships with the app at
  `Tabrok.app/Contents/Resources/LICENSE.electron.txt`.
- **Chromium** — BSD-3-Clause with additional notices. The complete notices ship with the app at
  `Tabrok.app/Contents/Resources/LICENSES.chromium.html` (see `THIRD-PARTY-LICENSES/frameworks/chromium-README.txt`).
- **Playwright** — Apache-2.0 — Copyright (c) Microsoft Corporation — drives the bundled Chromium.
- **PyInstaller** — GPL-2.0-or-later with a special exception that permits building and distributing
  non-free (including commercial) programs. Your own code is unaffected.

## 2. Browser Automation

- **browser-use 0.13.10** — MIT License — Copyright (c) Gregor Zunic. Shipped unmodified; Tabrok applies
  its fixes as in-memory runtime patches at process startup (see `backend/services/browser_engine.py`),
  so no modified third-party source is redistributed.

## 3. Bundled Python Packages (frozen into `tabrok-backend`) — 159 packages

Versions pinned in `backend/requirements.lock.txt`:

- **aiofiles 25.1.0** — Apache-2.0
- **aiohappyeyeballs 2.7.1** — PSF-2.0
- **aiohttp 3.14.3** — Apache-2.0 AND MIT
- **aiosignal 1.4.0** — Apache 2.0
- **altgraph 0.17.5** — MIT
- **annotated-doc 0.0.5** — MIT
- **annotated-types 0.8.0** — see THIRD-PARTY-LICENSES/
- **anthropic 0.76.0** — MIT
- **anyio 4.14.2** — MIT
- **attrs 26.1.0** — MIT
- **backoff 2.2.1** — MIT
- **beautifulsoup4 4.15.0** — MIT License
- **boolean.py 5.0** — see THIRD-PARTY-LICENSES/
- **browser-harness 0.1.13** — MIT (browser-use distribution)
- **browser-use 0.13.10** — see THIRD-PARTY-LICENSES/
- **browser-use-sdk 3.4.2** — MIT
- **bubus 1.5.6** — see THIRD-PARTY-LICENSES/
- **CacheControl 0.14.4** — see THIRD-PARTY-LICENSES/
- **cdp-use 1.4.5** — MIT
- **certifi 2026.7.22** — MPL-2.0
- **cffi 2.1.1** — MIT
- **charset-normalizer 3.5.1** — MIT
- **click 8.3.3** — BSD-3-Clause
- **cloudpickle 3.1.2** — BSD-3-Clause
- **cryptography 50.0.1** — Apache-2.0 OR BSD-3-Clause
- **cyclonedx-python-lib 11.12.0** — Apache-2.0
- **Cython 3.3.0** — see THIRD-PARTY-LICENSES/
- **defusedxml 0.7.1** — PSFL
- **distro 1.9.0** — Apache License, Version 2.0
- **docstring_parser 0.18.0** — MIT
- **fastapi 0.141.1** — MIT
- **fetch-use 0.4.0** — MIT
- **filelock 4.1.1** — see THIRD-PARTY-LICENSES/
- **filetype 1.2.0** — MIT
- **frozenlist 1.8.0** — Apache-2.0
- **google-api-core 2.29.0** — Apache 2.0
- **google-api-python-client 2.188.0** — Apache 2.0
- **google-auth 2.48.0** — Apache 2.0
- **google-auth-httplib2 0.4.2** — Apache 2.0
- **google-auth-oauthlib 1.2.4** — Apache 2.0
- **google-genai 1.65.0** — Apache-2.0
- **googleapis-common-protos 1.75.3** — Apache-2.0
- **greenlet 3.5.6** — MIT
- **groq 1.0.0** — Apache-2.0
- **h11 0.16.0** — MIT
- **httpcore 1.0.9** — see THIRD-PARTY-LICENSES/
- **httpcore2 2.13.0** — see THIRD-PARTY-LICENSES/
- **httplib2 0.32.0** — MIT
- **httpx 0.28.1** — BSD-3-Clause
- **httpx2 2.13.0** — see THIRD-PARTY-LICENSES/
- **idna 3.20** — BSD-3-Clause
- **iniconfig 2.3.0** — MIT
- **inquirerpy 0.3.4** — MIT
- **jiter 0.17.0** — MIT
- **jsonpatch 1.33** — Modified BSD License
- **jsonpointer 3.1.1** — Modified BSD License
- **jsonschema 4.26.0** — MIT
- **jsonschema-specifications 2025.9.1** — MIT
- **langchain 1.4.3** — MIT
- **langchain-core 1.6.6** — MIT
- **langchain-google-genai 4.4.0** — MIT
- **langchain-openai 1.3.4** — MIT
- **langchain-protocol 0.0.19** — MIT
- **langgraph 1.2.12** — MIT
- **langgraph-checkpoint 4.2.0** — MIT
- **langgraph-prebuilt 1.1.0** — MIT
- **langgraph-sdk 0.4.5** — MIT
- **langsmith 0.14.2** — MIT
- **license-expression 30.4.4** — Apache-2.0
- **lxml 6.1.3** — BSD-3-Clause
- **macholib 1.16.4** — MIT
- **markdown-it-py 4.2.0** — see THIRD-PARTY-LICENSES/
- **markdownify 1.2.2** — see THIRD-PARTY-LICENSES/
- **mcp 2.1.1** — MIT
- **mcp-types 2.1.1** — MIT
- **mdurl 0.1.2** — see THIRD-PARTY-LICENSES/
- **msgpack 1.2.3** — Apache-2.0
- **multidict 6.9.0** — Apache License 2.0
- **oauthlib 3.3.1** — BSD-3-Clause
- **ollama 0.6.1** — MIT
- **openai 2.26.0** — Apache-2.0
- **opentelemetry-api 1.44.0** — Apache-2.0
- **orjson 3.12.0** — see THIRD-PARTY-LICENSES/
- **ormsgpack 1.12.2** — see THIRD-PARTY-LICENSES/
- **packageurl-python 0.17.6** — MIT
- **packaging 26.3** — Apache-2.0 OR BSD-2-Clause
- **pfzy 0.3.4** — MIT
- **pillow 12.3.0** — MIT-CMU
- **platformdirs 4.13.0** — see THIRD-PARTY-LICENSES/
- **playwright 1.63.0** — Apache-2.0
- **pluggy 1.6.0** — MIT
- **portalocker 4.4.0** — BSD-3-Clause
- **posthog 7.7.0** — MIT
- **prompt_toolkit 3.0.53** — see THIRD-PARTY-LICENSES/
- **propcache 0.5.4** — Apache-2.0
- **proto-plus 1.28.4** — Apache 2.0
- **protobuf 6.33.6** — 3-Clause BSD License
- **psutil 7.2.2** — BSD-3-Clause
- **py-serializable 2.1.0** — Apache-2.0
- **pyasn1 0.6.4** — BSD-2-Clause
- **pyasn1_modules 0.4.2** — BSD
- **pycparser 3.0** — see THIRD-PARTY-LICENSES/
- **pydantic 2.13.5** — MIT
- **pydantic-settings 2.15.0** — see THIRD-PARTY-LICENSES/
- **pydantic_core 2.46.5** — MIT
- **pyee 13.0.1** — MIT
- **Pygments 2.21.0** — see THIRD-PARTY-LICENSES/
- **pyinstaller 6.22.3** — GPLv2-or-later with a special exception which allows to use PyInstaller to build and distribute non-free programs (including commercial ones)
- **pyinstaller-hooks-contrib 2026.7** — see THIRD-PARTY-LICENSES/
- **PyJWT 2.15.0** — see THIRD-PARTY-LICENSES/
- **pyobjc-core 12.2.2** — MIT
- **pyobjc-framework-Cocoa 12.2.2** — see THIRD-PARTY-LICENSES/
- **pyotp 2.9.0** — MIT License
- **pyparsing 3.3.2** — MIT
- **pypdf 6.19.0** — BSD-3-Clause
- **pytest 9.1.1** — MIT
- **pytest-asyncio 1.4.0** — Apache-2.0
- **python-dateutil 2.9.0.post0** — Dual License
- **python-docx 1.2.0** — MIT
- **python-dotenv 1.2.2** — BSD-3-Clause
- **python-multipart 0.0.32** — see THIRD-PARTY-LICENSES/
- **PyYAML 6.0.3** — see THIRD-PARTY-LICENSES/
- **referencing 0.37.0** — MIT
- **regex 2026.9.29** — Apache-2.0
- **reportlab 4.4.9** — BSD license (see license.txt for details), Copyright (c) 2000-2025, ReportLab Inc.
- **requests 2.33.0** — Apache-2.0
- **requests-oauthlib 2.0.0** — ISC
- **requests-toolbelt 1.0.0** — Apache 2.0
- **rich 14.3.3** — MIT
- **rpds-py 2026.6.3** — MIT
- **rsa 4.9.1** — Apache-2.0
- **screeninfo 0.8.1** — MIT
- **sentry-sdk 2.71.0** — MIT
- **setuptools 84.0.0** — MIT
- **six 1.17.0** — MIT
- **sniffio 1.3.1** — MIT OR Apache-2.0
- **sortedcontainers 2.4.0** — Apache 2.0
- **soupsieve 2.9.2** — see THIRD-PARTY-LICENSES/
- **sse-starlette 3.4.11** — BSD-3-Clause
- **starlette 1.6.0** — BSD-3-Clause
- **structlog 26.1.0** — see THIRD-PARTY-LICENSES/
- **tenacity 9.1.4** — Apache 2.0
- **tiktoken 0.14.0** — MIT License
- **tomli 2.5.0** — MIT
- **tomli_w 1.2.0** — see THIRD-PARTY-LICENSES/
- **tqdm 4.70.1** — MPL-2.0 AND MIT
- **truststore 0.10.4** — MIT
- **typing-inspection 0.4.4** — MIT
- **typing_extensions 4.15.0** — PSF-2.0
- **uritemplate 4.2.0** — BSD 3-Clause OR Apache-2.0
- **urllib3 2.8.0** — MIT
- **uuid7 0.1.0** — MIT license
- **uuid_utils 0.17.1** — MIT
- **uvicorn 0.53.0** — BSD-3-Clause
- **wcwidth 0.8.4** — MIT
- **websockets 15.0.1** — BSD-3-Clause
- **xxhash 4.0.1** — BSD-2-Clause
- **yarl 1.25.1** — Apache-2.0
- **zstandard 0.25.0** — BSD-3-Clause (BSD-3-Clause elected from dual BSD/GPL)

All packages above are under permissive licenses (MIT, BSD, Apache-2.0, ISC, PSF) or the
weak file-level copyleft of MPL-2.0 (certifi, tqdm) **without modification**; none places
Tabrok's own code under any copyleft obligation.

## 4. Bundled npm Packages (inside `app.asar` and the main process)

Production dependencies declared in `frontend/package.json` (full transitive tree in `THIRD-PARTY-LICENSES/npm/`):

- **@radix-ui/react-dialog 1.1.23** — MIT
- **@radix-ui/react-label 2.1.16** — MIT
- **@radix-ui/react-select 2.4.1** — MIT
- **@radix-ui/react-slot 1.3.3** — MIT
- **@radix-ui/react-toast 1.2.23** — MIT
- **@sentry/electron 7.20.0** — MIT
- **@tailwindcss/vite 4.3.3** — MIT
- **adm-zip 0.6.1** — MIT
- **class-variance-authority 0.7.1** — Apache-2.0
- **clsx 2.1.1** — MIT
- **electron-updater 6.8.9** — MIT
- **lucide-react 1.57.0** — ISC
- **pino 10.3.1** — MIT
- **react 19.2.8** — MIT
- **react-dom 19.2.8** — MIT
- **tailwind-merge 1.14.0** — MIT
- **tailwindcss 4.3.3** — MIT
- **webfontloader 1.6.28** — Apache-2.0
- **ws 8.21.3** — MIT

All npm dependencies are permissively licensed (MIT, ISC, Apache-2.0, BSD). Notable transitive
runtime dependencies include `undici` (MIT), `@sentry/core` and the OpenTelemetry packages
(Apache-2.0/MIT as declared), Radix UI primitives (MIT), `ws` (MIT), `class-variance-authority`, 
`clsx`, `tailwind-merge` (MIT), and `webfontloader` (Apache-2.0).

## 5. Copied-In UI Components

- **shadcn/ui** — MIT License — Copyright (c) 2023 shadcn. The derived components in
  `frontend/src/components/ui/` (`dialog.tsx`, `dropdown-menu.tsx`, `label.tsx`, `scroll-area.tsx`,
  `separator.tsx`, `slider.tsx`, `textarea.tsx`, `tooltip.tsx`) are MIT-licensed copies incorporated
  per the shadcn/ui distribution model and carry the upstream MIT header. Other UI files
  (`button.tsx`, `card.tsx`, `input.tsx`, `select.tsx`, `toast.tsx`) are hand-written proprietary
  implementations and are not derived from shadcn/ui.

## 6. Fonts & Icons

- **lucide-react** — ISC License — Copyright (c) Lucide Contributors.
- **Nasalization** — display typeface (freeware); ships inside `app.asar` assets.

## 7. Runtime Modification Notice

Tabrok patches the *installed* `browser-use` package in memory at startup (URL-allow guarding,
detached-target resilience, and 503-retry handling). No modified third-party source file is
redistributed; upstream packages are shipped exactly as published.
