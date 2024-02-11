DNS Service for Networking Labs
===============================

A simple DNS service for networking labs. The service uses [Dnsmasq][Dnsmasq].

[Dnsmasq]: https://thekelleys.org.uk/dnsmasq/doc.html

Basic Usage
-----------

Specify IP addresses  and corresponding domain names in the `./hosts`
configuration file. The configuration syntax is the same as for the
[`/etc/hosts`][HostsManual] file.

[HostsManual]: https://man7.org/linux/man-pages/man5/hosts.5.html

Start the service:

```sh
docker compose up --detach
```

Print logs:

```sh
docker compose logs
```

Stop the service:

```sh
docker compose down
```

Testing
-------

Send a test DNS query:

```sh
dig @127.0.0.1 foo.example.com
```
