===================
Release Notes 1.0.x
===================

1.0.5
------------

* Fixed crash issue for Android
* Upgraded Javet engine pool to expose more statistics
* Upgraded Javet engine pool scheduling algorithm

1.0.4 V8 9.6
------------

* Upgraded Node.js to ``v16.13.0`` `(2021-10-26) <https://github.com/nodejs/node/blob/master/doc/changelogs/CHANGELOG_V16.md#16.13.0>`_
* Upgraded V8 to ``v9.6.180.8`` `(2021-10-25) <https://v8.dev/blog/v8-release-96>`_
* Added ``JavetBridgeConverter`` for completely bridging Java and JavaScript
* Fixed a potential core dump issue caused by memory allocation failure in V8
* Added error code 806 and ``JavetOutOfMemoryException``
* Upgraded ``JavetEnginePool`` to get away from busy-wait
* Added ``hasPendingException()``, ``hasPendingMessage()``, ``hasScheduledException()``, ``promoteScheduledException()`` and ``reportPendingMessages()`` to ``V8Runtime``

1.0.3 Android ABI 21
--------------------

* Supported Android (arm, arm64, x86 and x86_64) ABI >= 21
* Added ``addGCEpilogueCallback``, ``addGCPrologueCallback``, ``removeGCEpilogueCallback`` and ``removeGCPrologueCallback`` to ``V8Runtime``
* Enhanced ``JavetLibLoadingListener`` to take environment variables

1.0.2 First Time with Android
-----------------------------

* Supported Android (arm, arm64, x86 and x86_64) ABI >= 26
* Upgraded Node.js to ``v16.12.0`` `(2021-10-20) <https://github.com/nodejs/node/blob/master/doc/changelogs/CHANGELOG_V16.md#16.12.0>`_
* Upgraded V8 to ``v9.5.172.22`` `(2021-10-20) <https://v8.dev/blog/v8-release-95>`_
* Added ``V8Internal``
* Cleaned up ``V8Runtime`` internal API
* Removed ``MethodHandle`` for Android compatibility

1.0.1 Custom Library Loading
----------------------------

* Upgraded Node.js to ``v16.11.1`` `(2021-10-12) <https://github.com/nodejs/node/blob/master/doc/changelogs/CHANGELOG_V16.md#16.11.1>`_
* Upgraded V8 to ``v9.4.146.19`` `(2021-10-01) <https://v8.dev/blog/v8-release-94>`_
* Upgraded callback function and proxy converter to implicitly cast more primitive types
* Added ``IJavetLibLoadingListener`` and ``JavetLibLoadingListener`` to allow custom lib loading
* Fixed a potential memory leak introduced mistakenly in v1.0.0

1.0.0 First Time with Node.js v16
---------------------------------

* Upgraded Node.js to ``v16.10.0`` `(2021-09-22) <https://github.com/nodejs/node/blob/master/doc/changelogs/CHANGELOG_V16.md#16.10.0>`_
* Added ``V8RuntimeOptions`` and ``NodeRuntimeOptions``
* Added ``getV8HeapStatistics()``, ``getV8HeapSpaceStatistics()`` and ``getV8SharedMemoryStatistics()`` to ``V8Runtime``
