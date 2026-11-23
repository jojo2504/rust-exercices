# Rust Practice

My solutions for exercises from [100 Exercises to Learn Rust](https://rust-exercises.com/):

- **04 – Traits**, **05 – Ticket v2**, **06 – Ticket management**
- **07 – Threads**: all exercises (01–14)
  - Splitting work across threads: `thread::spawn`, `'static` slices, `Vec::leak`, scoped threads
  - Client/server ticket store over channels: `mpsc` channels, response channels (ack), a cloneable client, bounded channels (`sync_channel`, `try_send` + `OverloadedError`), patch updates
  - Interior mutability with `Rc<RefCell<_>>`
  - Shared state with `Arc<Mutex<_>>`, then `Arc<RwLock<_>>`, and finally dropping channels entirely
  - `Send` / `Sync`
- **08 – Futures**: exercises 00–07
  - Async TCP echo server with `tokio`
  - Concurrent tasks with `tokio::spawn`, sharing non-`Clone` data via `Arc`
  - Keeping futures `Send` (no `Rc` held across `.await`)
  - Offloading blocking I/O with `spawn_blocking`
  - Async-aware channels (`tokio::sync::mpsc`) to avoid deadlocks
  - Not done yet: 08 (outro)

Skipping the trivial ones and focused on exercises that gave me something to learn or practice.
