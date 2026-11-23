# Cross-Platform Benchmark Results

This branch records automated cross-platform `TestE2EMicroBench` latency and host CPU utilization results.

## Latest Summary by Platform and Backend

| Target | Backend | Commit | `host_new` | `getpid` | `open_close` | `pipe_pingpong` | `futex_pingpong` | `fork_wait` | `fork_exec_true` | `shm_sparse_idle` |
| :--- | :--- | :--- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| `linux/amd64` | `systrap` | `b14cfd64` | 1.45 ms | 2.8 us (103%) | 8.8 us (111%) | 15.3 us (112%) | 5.1 us (108%) | 1.79 ms (185%) | 413.4 us (125%) | 0.2% CPU |
| `linux/arm64` | `systrap` | `b14cfd64` | 2.46 ms | 3.1 us (102%) | 11.0 us (110%) | 17.1 us (113%) | 6.8 us (107%) | 2.00 ms (179%) | 744.4 us (117%) | 0.3% CPU |
| `windows/amd64` | `systrap` | `b14cfd64` | 60.68 ms | 603 ns (94%) | 5.2 us (115%) | 83.1 us (116%) | 69.5 us (116%) | 12.03 ms (110%) | 8.29 ms (79%) | 2.3% CPU |
| `windows/amd64` | `whpx` | `b14cfd64` | 10.12 ms | 16.6 us (102%) | 45.6 us (134%) | 163.5 us (200%) | 150.9 us (184%) | 1.82 ms (220%) | 1.71 ms (135%) | 0.0% CPU |
| `windows/arm64` | `systrap` | `b14cfd64` | 87.99 ms | 950 ns (90%) | 5.5 us (107%) | 35.1 us (127%) | 27.1 us (117%) | 16.53 ms (33%) | 17.99 ms (19%) | 1.6% CPU |

## Historical Trend (Last 10 Runs per Target)

### `linux/amd64` (`systrap`)

| Timestamp (UTC) | Commit | `getpid` | `pipe_pingpong` | `futex_pingpong` | `fork_wait` | `fork_exec_true` | `shm_sparse_idle` | Failures |
| :--- | :--- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| `2026-11-23T15:17:41Z` | `b14cfd64` | 2.8 us (103%) | 15.3 us (112%) | 5.1 us (108%) | 1.79 ms (185%) | 413.4 us (125%) | 0.2% CPU | 0 |

### `linux/arm64` (`systrap`)

| Timestamp (UTC) | Commit | `getpid` | `pipe_pingpong` | `futex_pingpong` | `fork_wait` | `fork_exec_true` | `shm_sparse_idle` | Failures |
| :--- | :--- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| `2026-11-23T15:17:41Z` | `b14cfd64` | 3.1 us (102%) | 17.1 us (113%) | 6.8 us (107%) | 2.00 ms (179%) | 744.4 us (117%) | 0.3% CPU | 0 |

### `windows/amd64` (`systrap`)

| Timestamp (UTC) | Commit | `getpid` | `pipe_pingpong` | `futex_pingpong` | `fork_wait` | `fork_exec_true` | `shm_sparse_idle` | Failures |
| :--- | :--- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| `2026-11-23T15:17:41Z` | `b14cfd64` | 603 ns (94%) | 83.1 us (116%) | 69.5 us (116%) | 12.03 ms (110%) | 8.29 ms (79%) | 2.3% CPU | 0 |

### `windows/amd64` (`whpx`)

| Timestamp (UTC) | Commit | `getpid` | `pipe_pingpong` | `futex_pingpong` | `fork_wait` | `fork_exec_true` | `shm_sparse_idle` | Failures |
| :--- | :--- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| `2026-11-23T15:17:41Z` | `b14cfd64` | 16.6 us (102%) | 163.5 us (200%) | 150.9 us (184%) | 1.82 ms (220%) | 1.71 ms (135%) | 0.0% CPU | 0 |

### `windows/arm64` (`systrap`)

| Timestamp (UTC) | Commit | `getpid` | `pipe_pingpong` | `futex_pingpong` | `fork_wait` | `fork_exec_true` | `shm_sparse_idle` | Failures |
| :--- | :--- | ---: | ---: | ---: | ---: | ---: | ---: | ---: |
| `2026-11-23T15:17:41Z` | `b14cfd64` | 950 ns (90%) | 35.1 us (127%) | 27.1 us (117%) | 16.53 ms (33%) | 17.99 ms (19%) | 1.6% CPU | 0 |

