# Memos – Self‑hosted note‑taking

This add‑on runs the open‑source **Memos** service (https://github.com/usememos/memos) inside Home Assistant.

## How to use

1. Install the add‑on and start it.
2. Open the web UI at `http://<HA_IP>:8080`.
3. Your notes are stored persistently under `/share/memos`.

## Options

| Option | Description | Default |
|--------|-------------|---------|
| `log_level` | Logging verbosity | `info` |
| `data_path` | Where to store notes on the host | `/share/memos` |
