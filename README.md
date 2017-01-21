# NAME

SMS::Send::Sergel::Simple::HTTP

# SYNOPSIS

    use SMS::Send;
    use SMS::Send::Sergel::Simple::HTTP;

    # Create sender
    my $sender = SMS::Send->new('Sergel::Simple::HTTP',
      _url       => 'API url'
      _serviceid => 'serviceid',
      _login     => 'username',
      _password  => 'password',
      _sender    => 'SENDER' # Text or phone number
    );

    # Send message, returns true if OK
    my $sent = $sender->send_sms(
      text => 'My message text',
      to => '+4612345678', # Phone number
    );

    if ($sent) {
      # OK
    } else {
      # Not OK
    }

# DESCRIPTION

SMS::Send::Sergel::Simple::HTTP is a perl library for
sending SMS with the Sergel Simple HTTP SMS service.

# AUTHOR

Eivin Giske Skaaren <eivin@sysmystic.com>

# COPYRIGHT

Copyright 2017- Eivin Giske Skaaren

# LICENSE

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# SEE ALSO
