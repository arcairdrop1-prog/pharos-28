# Pharos Event/Log Monitor Agent

An intelligent agent developed in **Java** for the Pharos Agent Arena designed to watch a Pharos contract for specific events (such as `Transfer` or `Deposit`) using Chain MCP, running continuously and reporting decoded events without duplicates.

## 📋 Requirements Met

1. **Filtered Log Queries (Req. 01):** Uses Chain MCP log queries filtered by contract address and event signature.
2. **Continuous Polling & Deduplication (Req. 02):** Runs continuously block-by-block and reports only new events, strictly avoiding duplicates.
3. **Decoded Readable Fields (Req. 03):** Decodes each event into readable fields including `from`, `to`, `amount`, `tx hash`, and `block`.
4. **Event Capture Demo (Req. 04):** Demonstrates catching live or test events successfully during polling cycles.

## 🚀 How to Run

1. Make sure you have **Java JDK** installed.
2. Compile the file:
   ```bash
   javac EventLogMonitor.java
