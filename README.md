Roster
=====

Create or delete system user accounts in Mac, Linux and Windows. 

API
---

    var roster = require('roster');

    roster.exists('username', function(exists) {
      console.log('User exists? ' + exists);
    })

    roster.create({ user: 'new_guy', full_name: 'The New Guy' }, function(err) {
      if (!err)
        console.log('Successfully created.')
    })

    roster.delete('bad_user', function(err) {
      if (!err)
        console.log('Successfully delete.')
    })

That's it.

Boring stuff
------------

Written by Tomás Pollak. MIT licensed.
