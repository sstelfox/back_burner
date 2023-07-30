# Back Burner

Back Burner is a flexible async background task queue and executor. Keep your
webservers fast by delaying the expensive operations to the background where
they can take their sweet time.

## Features

This project is currently an early work in progress and the APIs are heavily
under active development (Semantic versioning around breaking changes will be
followed). The following list of features is the wishlist that has roughly been
prioritized in order of intended development.

* [ ] Execution of enqueued tasks on a configurable number of workers
* [ ] Database backed task queue (Sqlite & PostgreSQL)
* [ ] Named queues with priorities
* [ ] Tower style middleware "Layers"
* [ ] Job error and panic handling, backoff, retries, and dead queue
* [ ] Configurable task history clean up (delete on success, delete after X time,
      always delete, keep last X)
* [ ] Recurring job scheduling
* [ ] Multiple worker pools with chosen named queues
* [ ] Independent task running binary
* [ ] Schedule only task library (schedule in your webserve, execute in your
      task runner)
* [ ] Expiring jobs
* [ ] Blocking task queues
* [ ] Unique per-job task enqueueing
* [ ] Unique per-job-and-arguments task enqueueing
* [ ] Job metrics collection
* [ ] "Dead" job hook (ran out of retries)
* [ ] Per-job retry configuration
* [ ] Per-job alternate queue/priority
* [ ] Batch job operations (collect a bunch of jobs into one, execute them in
      parallel, queue another job when they're all complete, set success/failure
      thresholds for batch processing).
* [ ] Concurrent Job Rate Limiting
* [ ] Job Bucket Time Based Rate Limiting
