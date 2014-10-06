### HipChat-Fail2Ban 

Fail2Ban action to send notifications to [HipChat](https://www.hipchat.com)

### Requirements

* Curl utility
* HTTP(S) access from your server to HipChat service

### Install

  * Clone repository
   
  * Copy files into `/etc/fail2ban` folder
  
  * Copy `jail.local.example` as `jail.local`, or put entire contents into already existent file (corresponding to categories)

### Configuration

* Fill global values of `hipchat_token` and `hipchat_room` (also you may override them per jail)

* Set `action   = %(action_hipchat)s` for your jail (if you haven't copied `jail.local` completely)
 
* Set proper logpath depending on your repository

* Customize everything on your wish ;-)

* Restart fail2ban service

### LICENSE

This work is provided under the MIT License
