# Single-node Druid

This is a single-node Druid Vagrant box. Use `vagrant up` to start up the box for the first time, and `vagrant provision` to re-provision the box. It takes less than 5 minutes when you run `vagrant up` for the first time.

This box is based on the "quickstart" configuration. It runs one instance of all Druid components (one historical node, one real-time node, etc). Druid cluster is resource hungry. For example, a very simple data indexing task from the Quickstart would demands a lot of memory. For that reason, this box is previsioned to use 8GM of memory.

The box is accessible via a static IP address `192.168.33.30`. The default Druid ports are also mapped to the host machine. This makes it easier to access Druid APIs and guis. For example, coordinator console can be access at `http://localhost:8090/console.html`.