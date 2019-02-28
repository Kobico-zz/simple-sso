# simple-sso
gigya SSO simple implementation for testing purpose

set hosts: (add to /etc/hosts file)

127.0.0.1	eu1-prefix.sso-child3.soa
</br>
127.0.0.1	eu1.sso-child2.soa
</br>
52.30.9.119	login.eu1-prefix.sso-child3.soa

on a local directory, run:
<br>
git clone https://github.com/Kobico/simple-sso.git && cd simple-sso && npm start

<br>

1] go to: http://eu1-prefix.sso-child3.soa:8080
<br>
expected: login/register form prompt
<br>

2] register
<br>
expected: first name and last name rendered
<br>

3] go to: http://eu1.sso-child2.soa:8080
<br>
expected: first name and last name rendered (login form does not prompt)

that mean: SSO is working

if something is not working as expected, please specify exactly what, and capture network traffic.

if you encounter any problem with setting up the environment, please write to me: kobi.cohen@sap.com
