******************
PeerPlaysWebsocket
******************

This class allows subscribe to push notifications from the PeerPlays
node.

.. code-block:: python

    from pprint import pprint
    from peerplaysapi.websocket import PeerPlaysWebsocket

    ws = PeerPlaysWebsocket(
        "wss://node.testnet.peerplays.eu",
        markets=[["1.3.0", "1.3.172"]],
        accounts=["xeroc"],
        objects=["2.0.x", "2.1.x"],
        on_market=pprint,
        on_account=print,
    )

    ws.run_forever()

Defintion
=========
.. autoclass:: peerplaysapi.websocket.PeerPlaysWebsocket
    :members:
    :undoc-members:
    :private-members:
    :special-members:
