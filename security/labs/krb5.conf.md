``` 
[logging]
 default = FILE:/var/log/krb5libs.log
 kdc = FILE:/var/log/krb5kdc.log
 admin_server = FILE:/var/log/kadmind.log


[libdefaults]
default_realm = MIHENN87.LOCAL
dns_lookup_kdc = false
dns_lookup_realm = false
ticket_lifetime = 86400
renew_lifetime = 604800
forwardable = true
default_tgs_enctypes = rc4-hmac
default_tkt_enctypes = rc4-hmac
permitted_enctypes = rc4-hmac
udp_preference_limit = 1
kdc_timeout = 3000

[realms]
MIHENN87.LOCAL = {
kdc = ec2-54-202-97-115.us-west-2.compute.amazonaws.com
admin_server = ec2-54-202-97-115.us-west-2.compute.amazonaws.com
}

```