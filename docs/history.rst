Version History
===============

`2.0.0`_ Apr 24, 2017
---------------------
- Move Mixin and AMQP client to separate files
- Replace AMQP connection handling code with latest internal version
- Provide ability to register callbacks for ready, unavailable, and persistent failure states
- Remove default AMQP URL from AMQP class, url is now a required parameter for install
- Rename amqp_publish 'message' parameter to 'body'
- Add properties for all AMQP states
- Provide mandatory AMQP properties (app_id, correlation_id, message_id, timestamp) automatically
    - Mandatory properties cannot be overridden
- Add unit test coverage for new functionality
    - Test execution requires a running AMQP server

`1.0.1`_ Feb 28, 2016
---------------------
- Fixed documentation links and generation.

`1.0.0`_ Mar 15, 2016
----------------------
- Connect to AMQP in ``sprockets.mixins.amqp.install`` and maintain and persist connection
- Change to use tornado locks.Condition vs locks.Event

`0.1.4`_ Mar 09, 2016
----------------------
- Reconnect in connection close callback

`0.1.3`_ Sept 28, 2015
----------------------
- Use packages instead of py_modules

`0.1.2`_ Sept 25, 2015
----------------------
- Don't log the message body

`0.1.1`_ Sept 24, 2015
----------------------
- Clean up installation and testing environment

`0.1.0`_ Sept 23, 2015
----------------------
 - Initial implementation

.. _Next Release: https://github.com/sprockets/sprockets.amqp/compare/2.0.0...HEAD
.. _2.0.0: https://github.com/sprockets/sprockets.amqp/compare/1.0.1...2.0.0
.. _1.0.1: https://github.com/sprockets/sprockets.amqp/compare/1.0.0...1.0.1
.. _1.0.0: https://github.com/sprockets/sprockets.amqp/compare/0.1.4...1.0.0
.. _0.1.4: https://github.com/sprockets/sprockets.amqp/compare/0.1.3...0.1.4
.. _0.1.3: https://github.com/sprockets/sprockets.amqp/compare/0.1.2...0.1.3
.. _0.1.2: https://github.com/sprockets/sprockets.amqp/compare/0.1.1...0.1.2
.. _0.1.1: https://github.com/sprockets/sprockets.amqp/compare/0.1.0...0.1.1
.. _0.1.0: https://github.com/sprockets/sprockets.amqp/compare/551982c...0.1.0
