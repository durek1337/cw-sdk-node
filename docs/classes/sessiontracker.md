[cw-sdk-node - v1.0.0-beta.9](../README.md) › [SessionTracker](sessiontracker.md)

# Class: SessionTracker

This class is used to keep trading sessions organized, and emit a ready status when the client
can trade.

## Hierarchy

* EventEmitter

  ↳ **SessionTracker**

## Index

### Constructors

* [constructor](sessiontracker.md#constructor)

### Properties

* [captureRejectionSymbol](sessiontracker.md#static-capturerejectionsymbol)
* [captureRejections](sessiontracker.md#static-capturerejections)
* [defaultMaxListeners](sessiontracker.md#static-defaultmaxlisteners)
* [errorMonitor](sessiontracker.md#static-errormonitor)

### Methods

* [addListener](sessiontracker.md#addlistener)
* [emit](sessiontracker.md#emit)
* [eventNames](sessiontracker.md#eventnames)
* [getMaxListeners](sessiontracker.md#getmaxlisteners)
* [isModuleReady](sessiontracker.md#ismoduleready)
* [isReady](sessiontracker.md#isready)
* [listenerCount](sessiontracker.md#listenercount)
* [listeners](sessiontracker.md#listeners)
* [off](sessiontracker.md#off)
* [on](sessiontracker.md#on)
* [once](sessiontracker.md#once)
* [prependListener](sessiontracker.md#prependlistener)
* [prependOnceListener](sessiontracker.md#prependoncelistener)
* [rawListeners](sessiontracker.md#rawlisteners)
* [removeAllListeners](sessiontracker.md#removealllisteners)
* [removeListener](sessiontracker.md#removelistener)
* [reset](sessiontracker.md#reset)
* [setMaxListeners](sessiontracker.md#setmaxlisteners)
* [setModuleReady](sessiontracker.md#setmoduleready)
* [listenerCount](sessiontracker.md#static-listenercount)
* [on](sessiontracker.md#static-on)
* [once](sessiontracker.md#static-once)

## Constructors

###  constructor

\+ **new SessionTracker**(`tradeSubs`: [TradeSubscription](../interfaces/tradesubscription.md)[]): *[SessionTracker](sessiontracker.md)*

*Overrides void*

*Defined in [src/websocket/SessionTracker.ts:25](https://github.com/cryptowatch/cw-sdk-node/blob/master/src/websocket/SessionTracker.ts#L25)*

**Parameters:**

Name | Type |
------ | ------ |
`tradeSubs` | [TradeSubscription](../interfaces/tradesubscription.md)[] |

**Returns:** *[SessionTracker](sessiontracker.md)*

## Properties

### `Static` captureRejectionSymbol

▪ **captureRejectionSymbol**: *keyof symbol*

*Inherited from void*

Defined in node_modules/@types/node/events.d.ts:38

___

### `Static` captureRejections

▪ **captureRejections**: *boolean*

*Inherited from void*

Defined in node_modules/@types/node/events.d.ts:44

Sets or gets the default captureRejection value for all emitters.

___

### `Static` defaultMaxListeners

▪ **defaultMaxListeners**: *number*

*Inherited from void*

Defined in node_modules/@types/node/events.d.ts:45

___

### `Static` errorMonitor

▪ **errorMonitor**: *keyof symbol*

*Inherited from void*

Defined in node_modules/@types/node/events.d.ts:37

This symbol shall be used to install a listener for only monitoring `'error'`
events. Listeners installed using this symbol are called before the regular
`'error'` listeners are called.

Installing a listener using this symbol does not change the behavior once an
`'error'` event is emitted, therefore the process will still crash if no
regular `'error'` listener is installed.

## Methods

###  addListener

▸ **addListener**(`event`: string | symbol, `listener`: function): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:569

**Parameters:**

▪ **event**: *string | symbol*

▪ **listener**: *function*

▸ (...`args`: any[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  emit

▸ **emit**(`event`: string | symbol, ...`args`: any[]): *boolean*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:579

**Parameters:**

Name | Type |
------ | ------ |
`event` | string &#124; symbol |
`...args` | any[] |

**Returns:** *boolean*

___

###  eventNames

▸ **eventNames**(): *Array‹string | symbol›*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:584

**Returns:** *Array‹string | symbol›*

___

###  getMaxListeners

▸ **getMaxListeners**(): *number*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:576

**Returns:** *number*

___

###  isModuleReady

▸ **isModuleReady**(`mID`: number, `m`: Module): *boolean*

*Defined in [src/websocket/SessionTracker.ts:56](https://github.com/cryptowatch/cw-sdk-node/blob/master/src/websocket/SessionTracker.ts#L56)*

**Parameters:**

Name | Type |
------ | ------ |
`mID` | number |
`m` | Module |

**Returns:** *boolean*

___

###  isReady

▸ **isReady**(): *boolean*

*Defined in [src/websocket/SessionTracker.ts:41](https://github.com/cryptowatch/cw-sdk-node/blob/master/src/websocket/SessionTracker.ts#L41)*

**Returns:** *boolean*

___

###  listenerCount

▸ **listenerCount**(`type`: string | symbol): *number*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:580

**Parameters:**

Name | Type |
------ | ------ |
`type` | string &#124; symbol |

**Returns:** *number*

___

###  listeners

▸ **listeners**(`event`: string | symbol): *Function[]*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:577

**Parameters:**

Name | Type |
------ | ------ |
`event` | string &#124; symbol |

**Returns:** *Function[]*

___

###  off

▸ **off**(`event`: string | symbol, `listener`: function): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:573

**Parameters:**

▪ **event**: *string | symbol*

▪ **listener**: *function*

▸ (...`args`: any[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  on

▸ **on**(`event`: string | symbol, `listener`: function): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:570

**Parameters:**

▪ **event**: *string | symbol*

▪ **listener**: *function*

▸ (...`args`: any[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  once

▸ **once**(`event`: string | symbol, `listener`: function): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:571

**Parameters:**

▪ **event**: *string | symbol*

▪ **listener**: *function*

▸ (...`args`: any[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  prependListener

▸ **prependListener**(`event`: string | symbol, `listener`: function): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:582

**Parameters:**

▪ **event**: *string | symbol*

▪ **listener**: *function*

▸ (...`args`: any[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  prependOnceListener

▸ **prependOnceListener**(`event`: string | symbol, `listener`: function): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:583

**Parameters:**

▪ **event**: *string | symbol*

▪ **listener**: *function*

▸ (...`args`: any[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  rawListeners

▸ **rawListeners**(`event`: string | symbol): *Function[]*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:578

**Parameters:**

Name | Type |
------ | ------ |
`event` | string &#124; symbol |

**Returns:** *Function[]*

___

###  removeAllListeners

▸ **removeAllListeners**(`event?`: string | symbol): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:574

**Parameters:**

Name | Type |
------ | ------ |
`event?` | string &#124; symbol |

**Returns:** *this*

___

###  removeListener

▸ **removeListener**(`event`: string | symbol, `listener`: function): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:572

**Parameters:**

▪ **event**: *string | symbol*

▪ **listener**: *function*

▸ (...`args`: any[]): *void*

**Parameters:**

Name | Type |
------ | ------ |
`...args` | any[] |

**Returns:** *this*

___

###  reset

▸ **reset**(): *void*

*Defined in [src/websocket/SessionTracker.ts:60](https://github.com/cryptowatch/cw-sdk-node/blob/master/src/websocket/SessionTracker.ts#L60)*

**Returns:** *void*

___

###  setMaxListeners

▸ **setMaxListeners**(`n`: number): *this*

*Inherited from void*

Defined in node_modules/@types/node/globals.d.ts:575

**Parameters:**

Name | Type |
------ | ------ |
`n` | number |

**Returns:** *this*

___

###  setModuleReady

▸ **setModuleReady**(`mID`: number, `m`: Module): *void*

*Defined in [src/websocket/SessionTracker.ts:45](https://github.com/cryptowatch/cw-sdk-node/blob/master/src/websocket/SessionTracker.ts#L45)*

**Parameters:**

Name | Type |
------ | ------ |
`mID` | number |
`m` | Module |

**Returns:** *void*

___

### `Static` listenerCount

▸ **listenerCount**(`emitter`: EventEmitter, `event`: string | symbol): *number*

*Inherited from void*

Defined in node_modules/@types/node/events.d.ts:26

**`deprecated`** since v4.0.0

**Parameters:**

Name | Type |
------ | ------ |
`emitter` | EventEmitter |
`event` | string &#124; symbol |

**Returns:** *number*

___

### `Static` on

▸ **on**(`emitter`: EventEmitter, `event`: string): *AsyncIterableIterator‹any›*

*Inherited from void*

Defined in node_modules/@types/node/events.d.ts:23

**Parameters:**

Name | Type |
------ | ------ |
`emitter` | EventEmitter |
`event` | string |

**Returns:** *AsyncIterableIterator‹any›*

___

### `Static` once

▸ **once**(`emitter`: NodeEventTarget, `event`: string | symbol): *Promise‹any[]›*

*Inherited from void*

*Overrides void*

Defined in node_modules/@types/node/events.d.ts:21

**Parameters:**

Name | Type |
------ | ------ |
`emitter` | NodeEventTarget |
`event` | string &#124; symbol |

**Returns:** *Promise‹any[]›*
