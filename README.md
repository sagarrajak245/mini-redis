
### MiniRedis (C++ In-Memory Database)

**In-Memory Redis-like Key-Value Store (C++ Project)**
Designed and implemented a Redis-inspired in-memory database supporting strings, lists, and hashes with disk persistence. Built custom TTL-based key expiration, flush-all, and rename capabilities. Enabled robust concurrency using mutex locks for safe multi-threaded access. Implemented DUMP/LOAD for persistent state restoration. Covered full CRUD operations and advanced indexing for lists and hashes.

---



**Overview**
This project is a simplified in-memory key-value database server inspired by Redis, built in C++. It supports a subset of Redis features, including data persistence and concurrent access handling.

---

### 🚀 Features

#### 🔑 Key-Value Store (Strings)

* `SET`, `GET`, `DELETE`: Basic key-value operations
* `EXPIRE`: Time-to-live for keys with automatic deletion
* `KEYS`, `TYPE`, `RENAME`: Utility commands to explore and manage data types

#### 📜 List Operations

* `LPUSH`, `RPUSH`, `LPOP`, `RPOP`: List-end manipulation
* `LLEN`, `LGET`, `LINDEX`, `LSET`, `LREM`: Full list access and modification

#### 🧱 Hash Operations

* `HSET`, `HGET`, `HEXISTS`, `HDEL`, `HGETALL`
* `HKEYS`, `HVALS`, `HLEN`, `HMSET`: Comprehensive hash map support

#### 💾 Persistence

* `DUMP`: Save database state to a disk file
* `LOAD`: Restore database from file

#### 🔁 Concurrency

* All commands are thread-safe using mutexes

#### ⏱️ Expiration

* TTL-based expiration support, purging keys on access

#### 🧹 Admin

* `FLUSHALL`: Clear entire database

---

### 🛠 Tech Stack

* **Language**: C++17
* **Concurrency**: `std::mutex`, thread-safe operations
* **Persistence**: Custom text-based file storage

---

Let me know if you want a `Usage` section, architecture diagram, or setup instructions added to the README!
