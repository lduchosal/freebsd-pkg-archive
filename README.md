# freebsd-pkg-archive

Archive of FreeBSD binary packages that are no longer available from the
official `pkg.freebsd.org` repositories, kept for pinned deployments.

Each package is published as a **GitHub release asset** (one release per
package version), never committed to git. Verify the SHA-256 before installing.

| Release | Package | ABI | SHA-256 | Why |
|---|---|---|---|---|
| `kibana8-8.11.3_1` | `kibana8-8.11.3_1.pkg` | FreeBSD:14:amd64 | `cd9666b15111ad9385b1d6a550e0c42d80021f22bc4149e73c64231509b29b57` | Must match Elasticsearch 8.11.3 (`textproc/elasticsearch8` port is still 8.11.3); `textproc/kibana8` jumped to 8.19.x, which refuses ES 8.11. Requires `node20`. |

## Licensing

Packages are redistributed unmodified, as built by the FreeBSD ports
collection. Each package keeps its upstream license (Kibana 8.11.3:
Elastic License 2.0 — see `/usr/local/share/licenses/` once installed and
https://www.elastic.co/licensing/elastic-license).
