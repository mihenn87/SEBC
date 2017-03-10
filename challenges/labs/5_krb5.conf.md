## KRB5

```
# Configuration snippets may be placed in this directory as well
includedir /etc/krb5.conf.d/

[logging]
 default = FILE:/var/log/krb5libs.log
 kdc = FILE:/var/log/krb5kdc.log
 admin_server = FILE:/var/log/kadmind.log

[libdefaults]
 dns_lookup_realm = false
 ticket_lifetime = 24h
 renew_lifetime = 7d
 forwardable = true
 rdns = false
 default_realm = MIHENN87.ES
 default_ccache_name = KEYRING:persistent:%{uid}

[realms]
        MIHENN87.ES = {
        kdc = ip-172-31-2-93.eu-central-1.compute.internal
        admin_server = ip-172-31-2-93.eu-central-1.compute.internal
}

[domain_realm]
 .mihenn87.es = MIHENN87.ES
 mihenn87.es = MIHENN87.ES


```