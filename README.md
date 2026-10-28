# NeOmega releases

Compiled NeOmega runtime packages, checksums, signed release manifests and release notes. No source code lives here.

- Download a package for your platform from [Releases](https://github.com/OmineDev/neomega-releases/releases).
- `latest.json` describes the newest release; `latest.json.sig` is its ed25519 signature (base64). The programs verify it with the public key in [`release.pub`](release.pub) before using any URL or checksum.
- Mainland China mirror: `https://releases.wuxie233.com/neomega/latest.json` (same signature scheme, package URLs point at the mirror).

Programs check for new versions on their own and only report them (log line and `/v1/status.update`). Updating is explicit: `neomega-runtime-live update --yes`, with automatic rollback to the previous binary if the new one fails to start.
