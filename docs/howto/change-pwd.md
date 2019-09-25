# {{ site.cluster.name }} Credentials

## Change password

To change your {{ site.cluster.name }} credentials, log into the cluster and call `passwd` from one of the _login_ nodes, e.g.

```sh
[alice@{{ site.login.name }} ~]$ passwd
Changing password for user alice.
Kerberos 5 Password: 
New password: 
Retype new password: 
passwd: all authentication tokens updated successfully.
[alice@{{ site.login.name }} ~]$ 
```

Only passwords adhering to the Unified [UCSF Enterprise Password Standard] are accepted.  Attempts to update to an insufficient password will produce an informative error message.

Alternatively, you can change your password using the [RBVI Kerberos Web Interface].

<div class="alert alert-warning" role="alert">
<strong>Please wait 5-10 minutes before attempting to login with your new password.</strong>  This is because it takes up to 10 minutes before your new password has propagated to all machines on the cluster.
</div>


## Verify credentials

To test your {{ site.cluster.name }} credentials, try to [login to {{ site.cluster.name }} via SSH]({{ '/get-started/access-cluster.html' | relative_url }}).  Alternatively, verify them from your browser:

1. Go to [https://www.cgl.ucsf.edu/admin/kerbtest.py](https://www.cgl.ucsf.edu/admin/kerbtest.py) in your browser.  A popup panel titled 'Sign in https://www.cgl.ucsf.edu' is opened by the browser.

3. Enter your {{ site.cluster.name }} login credentials in the two fields 'Username' and 'Password' and click 'Sign in'.

4. If you entered correct credentials, you will get to a confirmation page saying so.  If you entered incorrect credentials, there will be no error message and the popup will appear again.


## Reset password

To reset your _{{ site.cluster.name }}_ password, contact the admins at [wynton_admin@ucsf.edu]([wynton_admin@ucsf.edu).

<div class="alert alert-danger" role="alert" style="margin-top: 3ex">
<strong>Account are personal and login credentials must not be shared with others</strong>. If detected, access to the account will be automatically disabled.  It is still possible and easy for multiple users to share and collaborate on the same folders and scripts.  Don't hesitate to ask if you don't know how to do this - we're here to help.
</div>


[RBVI Kerberos web interface]: https://www.cgl.ucsf.edu/admin/chpass.py
[UCSF Enterprise Password Standard]: https://wiki.library.ucsf.edu/pages/viewpage.action?spaceKey=ITSI&title=Unified+UCSF+Enterprise+Password+Standard
