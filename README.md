Satan
=====

Create or delete system user accounts in Mac, Linux and Windows. 
The 'God' package name was taken so I said Ok, what the hell.

API
---

    var satan = require('satan');

    satan.exists('username', function(exists) {
      console.log('User exists? ' + exists);
    })

    satan.create({ user: 'new_guy', full_name: 'The New Guy' }, function(err) {
      if (!err)
        console.log('Successfully created.')
    })

    satan.delete('bad_user', function(err) {
      if (!err)
        console.log('Successfully delete.')
    })

That's it.

Boring stuff
------------

Written by Tomás Pollak. MIT licensed.