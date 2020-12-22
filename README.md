# fdb

### Beat version is live now
### This is a state manager and much more.


## Setup

### JS
<script src="./fdb.js"></script>

### TS
import * as fdb from './fdb';


## Simple Configuration 
fdb.config({storeName: 'app'});

## Usage

### To store a avlue in virtual DB
fdb.store('key', value);

### To retrive a value
fdb.store('key');

### Sync with localstorage
#### This needs to be used only one time for a key. Next time it will do the sync automatically
fdb.store('key', value, true); 

### Search data
fdb.store('key').search({key: value});
fdb.search({key: value});
