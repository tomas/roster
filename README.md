Roster
=====

Create or delete system user accounts in Mac, Linux and Windows. 

## Installation

    npm install roster

## API

    var roster = require('roster');

    roster.exists('username', function(exists) {
      console.log('User exists? ' + exists);
    })

    roster.create({ user: 'new_guy', name: 'The New Guy' }, function(err) {
      if (!err)
        console.log('Successfully created.')
    })

    roster.delete('old_user', function(err) {
      if (!err)
        console.log('Successfully deleted.')
    })

That's it. For all options, check the examples.

## Boring stuff

Written by Tomás Pollak. MIT licensed.
