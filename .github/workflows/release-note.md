```
Zenoh Dissector v${PKG_VER}
```

## Installation

Download and extract the corresponding zip file

### Linux

```bash
mkdir -p ~/.local/lib/wireshark/plugins/4.0/epan
cp libzenoh_dissector.so ~/.local/lib/wireshark/plugins/4.0/epan/libzenoh_dissector.so
```

### macOS

```bash
mkdir -p ~/.local/lib/wireshark/plugins/4-0/epan
cp libzenoh_dissector.dylib ~/.local/lib/wireshark/plugins/4-0/epan/libzenoh_dissector.so
```

### Windows

```powershell
\$epan_dir = "\$Env:APPDATA\Wireshark\plugins\4.0\epan"
if (-Not (Test-Path \$epan_dir)) {
    mkdir -p \$epan_dir
}
cp zenoh_dissector.dll \$epan_dir
```
