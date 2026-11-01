# Scoop bucket for NullWire-MCP

Scoop manifest for [NullWire-MCP](https://github.com/VoxNode-ux/nullwire-mcp), a RAM-only traffic inspector for AI assistants that scrubs secrets before the model sees them.

## Install

```powershell
scoop bucket add nullwire https://github.com/VoxNode-ux/scoop-nullwire
scoop install nullwire-mcp
nullwire-mcp install --client all --dry-run   # preview client changes
nullwire-mcp install --client all             # then register with your clients
```

## Update

```powershell
scoop update nullwire-mcp
```

## Uninstall

Remove NullWire from your MCP clients first, because Scoop doesn't touch those config files:

```powershell
nullwire-mcp install --uninstall --client all
scoop uninstall nullwire-mcp
```

## Supported platforms

Windows x86-64 and ARM64. Other platforms are available as prebuilt binaries on the [releases page](https://github.com/VoxNode-ux/nullwire-mcp/releases).

## Notes

- This bucket contains only the manifest. The program's source and documentation live in the main repository.
- Scoop checks each download against the SHA-256 hash in the manifest, which comes from the release's `SHA256SUMS.txt`.
 
