# --------------------------------------------------------------
# Base image – official Memos build (multi‑arch)
# --------------------------------------------------------------
FROM neosmemo/memos:latest

# --------------------------------------------------------------
# Create a directory for persistent data
# --------------------------------------------------------------
RUN mkdir -p /data && chown -R nobody:nogroup /data

# --------------------------------------------------------------
# Set the working directory
# --------------------------------------------------------------
WORKDIR /app

# --------------------------------------------------------------
# Entrypoint – the upstream image already starts the server,
# we just need to ensure the data dir is used.
# --------------------------------------------------------------
ENV MEMOS_DATA_DIR=${DATA_PATH:-/data}
ENV MEMOS_PORT=${MEMOS_PORT:-8080}

EXPOSE ${MEMOS_PORT}