API Reference
=============

.. module:: jwt

.. autofunction:: encode(payload, key, algorithm="HS256", headers=None, json_encoder=None) -> str

.. autofunction:: decode_complete(jwt, key="", algorithms=None, options=None, verify=None, detached_payload=None, audience=None, issuer=None, subject=None, leeway=0) -> dict[str, typing.Any]

.. autofunction:: decode(jwt, key="", algorithms=None, options=None, audience=None, issuer=None, leeway=0) -> dict[str, typing.Any]

.. autoclass:: PyJWT
    :class-doc-from: init
    :members:

.. autoclass:: PyJWK
    :class-doc-from: init
    :members:

    .. property:: algorithm_name

        :type: str

        The name of the algorithm used by the key.

    .. property:: Algorithm

        The :py:class:`Algorithm` class associated with the key.

.. autoclass:: PyJWKSet
    :class-doc-from: init
    :members:

.. autoclass:: PyJWKClient
    :class-doc-from: init
    :members:

.. note:: TODO: Finish documenting PyJWS class
.. module:: jwt.api_jws

.. autoclass:: jwt.api_jws.PyJWS
    :members:

Algorithms
----------

.. automodule:: jwt.algorithms
    :members: Algorithm

.. currentmodule:: jwt.algorithms

.. py:data:: AllowedPrivateKeys

    Type alias for private key objects accepted by asymmetric algorithms.

.. py:data:: AllowedPublicKeys

    Type alias for public key objects accepted by asymmetric algorithms.

.. currentmodule:: jwt


Types
----------

.. module:: jwt.types
    :synopsis: Type validation used in the JWT API
.. autoclass:: jwt.types.SigOptions
    :members:
    :undoc-members:
.. autoclass:: jwt.types.Options
    :members:
    :undoc-members:

Warnings
----------

.. automodule:: jwt.warnings
    :members:
    :show-inheritance:

Exceptions
----------

.. automodule:: jwt.exceptions
    :members:
    :inherited-members:
    :show-inheritance:
