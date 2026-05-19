# 1.2

`spawner.spawn()` only *creates* and *queues* the task, not run it. The task runs when `executor.run()` is called. `println!("Val's Computer: hey hey")` is a normal line with nothing special. The line is placed *before* `executor.run()`, that's why it is called first before the spawned task is executed.
