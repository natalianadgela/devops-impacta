Apache HTTP Server -

2.4.27 Released - Ultima versão.

Notas da Ultima Atualização:

Changes with Apache 2.4.27

*) SECURITY: CVE-2017-9789 (cve.mitre.org) mod_http2: Read after free. When under stress, closing many connections, the HTTP/2 handling code would sometimes access memory after it has been freed, resulting in potentially erratic behaviour. [Stefan Eissing]

*) SECURITY: CVE-2017-9788 (cve.mitre.org) mod_auth_digest: Uninitialized memory reflection. The value placeholder in [Proxy-]Authorization headers type 'Digest' was not initialized or reset before or between successive key=value assignments. [William Rowe]

*) COMPATIBILITY: mod_lua: Remove the undocumented exported 'apr_table' global variable when using Lua 5.2 or later. This was exported as a side effect from luaL_register, which is no longer supported as of Lua 5.2 which deprecates pollution of the global namespace. [Rainer Jung]

*) COMPATIBILITY: mod_http2: Disable and give warning when using Prefork. The server will continue to run, but HTTP/2 will no longer be negotiated. [Stefan Eissing]

*) COMPATIBILITY: mod_proxy_fcgi: Revert to 2.4.20 FCGI behavior for the default ProxyFCGIBackendType, fixing a regression with PHP-FPM. PR 61202. [Jacob Champion, Jim Jagielski]

*) mod_lua: Improve compatibility with Lua 5.1, 5.2 and 5.3. PR58188, PR60831, PR61245. [Rainer Jung]

*) mod_http2: Simplify ready queue, less memory and better performance. Update mod_http2 version to 1.10.7. [Stefan Eissing]

*) Allow single-char field names inadvertently disallowed in 2.4.25. PR 61220. [Yann Ylavic]

*) htpasswd / htdigest: Do not apply the strict permissions of the temporary passwd file to a possibly existing passwd file. PR 61240. [Ruediger Pluem]

*) core: Avoid duplicate HEAD in Allow header. This is a regression in 2.4.24 (unreleased), 2.4.25 and 2.4.26. PR 61207. [Christophe Jaillet]

2.2.34 Released End-of-Life - Penúltima versão.



NGINX -

nginx-1.13.4 - Ultima versão.

The ngx_http_mirror_module module (1.13.4) implements mirroring of an original request by creating background mirror subrequests. The output of mirror subrequests is ignored

nginx-1.13.3 - Penúltima versão.


WordPress -

WordPress 4.8.1 Maintenance Release - Ultima versão.

This release contains 29 maintenance fixes and enhancements, chief among them are fixes to the rich Text widget and the introduction of the Custom HTML widget. For a full list of changes, consult the release notes, the tickets closed, and the list of changes.

WordPress 4.8 “Evans” - Penúltima versão.


